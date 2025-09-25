## Pembuatan form tambah kendaraan

1. Buat file baru : `resources/views/admin/tambah_kendaraan.blade.php`
2. Isikan file tersebut dengan kode berikut
   ```html
    @extends('layouts.admin')
    @section('content')
    <main class="flex-1 p-6">
        <h1 class="text-3xl font-semibold">
            Dashboard
        </h1>
    
        <form class="bg-white shadow-md rounded px-8 pt-6 pb-8 mb-4 mt-4" action="{{ route('admin.kendaraan.store') }}" method="POST" enctype="multipart/form-data">
            @csrf
            <div class="mb-4">
                <label class="block text-gray-700 text-sm font-bold mb-2" for="nama">
                    Nama Kendaraan
                </label>
                <input
                    class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
                    name="nama" type="text" placeholder="Masukkan nama kendaraan">
            </div>
            <div class="mb-4">
                <label class="block text-gray-700 text-sm font-bold mb-2" for="harga">
                    Harga
                </label>
                <input
                    class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
                    name="harga" type="number" placeholder="Masukkan harga">
            </div>
            <div class="mb-4">
                <label class="block text-gray-700 text-sm font-bold mb-2" for="gambar">
                    Gambar
                </label>
                <input
                    class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
                    name="gambar" type="file">
            </div>
            <div class="mb-4">
                <button
                    class="bg-purple-800 hover:bg-purple-700 text-white font-bold py-2 px-4 rounded focus:outline-none focus:shadow-outline"
                    type="submit">
                    Tambah Kendaraan
                </button>
            </div>
        </form>
    </main>
    @endsection
   ```
3. Buat routes, buka file `routes/web.php` dan tambahkan baris berikut di paling bawah
    ```php
    Route::get('/admin/kendaraan/create', [KendaraanController::class, 'create'])
      ->middleware('auth')
      ->name('admin.kendaraan.create');
    ```
4. Buat fungsi/method baru pada file `app\Http\Controllers\KendaraanController.php`, beri nama fungsi tersebut dengan `create`
    ```php
    // kode lain diatas
    public function create()
    {
        return view('admin.tambah_kendaraan');
    }
    ```
5. Terakhir, tambahkan route yang kita buat ke tombol tambah kendaran pada file `resources\views\admin\kendaraan.blade.php`
    ```html
    {{-- kode lain diatas --}}
        <a href="{{ route('admin.kendaraan.create') }}" class="bg-purple-800 text-white px-2 py-1 mb-2 rounded inline-block">
            Tambah Kendaraan
        </a>
    {{-- kode lain dibawah --}}
    ```
## Membuat fungsionalitas tambah kendaraan dan menyimpan ke database
1. Buat model dan migration baru dengan menjalankan perintah berikut di git bash
    ```bash
    php artisan make:model Kendaraan -m
    ```

    Perintah diatas akan membuat model baru yang akan muncul di folder `app/Models` dan juga akan membuat migration baru yang akan muncul pada folder `database\migrations`
2. Selanjutnya kita edit file baru yang terbuat pada migration. `database\migrations\2025_09_25_220045_create_kendaraans_table.php` nama file mungkin akan berbeda karena terdapat tanggal dan detik pada awal file. pastikan yang diubah adalah file yang memiliki nama `kendaraans` sesuai nama model kita.
   Kode lengkap file yang sudah diedit sebagai berikut
   ```php
   <?php

    use Illuminate\Database\Migrations\Migration;
    use Illuminate\Database\Schema\Blueprint;
    use Illuminate\Support\Facades\Schema;
    
    return new class extends Migration
    {
        /**
         * Run the migrations.
         */
        public function up(): void
        {
            Schema::create('kendaraans', function (Blueprint $table) {
                $table->id();
                $table->string('name');
                $table->integer('harga');
                $table->string('gambar')->nullable();
                $table->timestamps();
            });
        }
    
        /**
         * Reverse the migrations.
         */
        public function down(): void
        {
            Schema::dropIfExists('kendaraans');
        }
    };

   ```
3. Edit file model `Kendaraan` kita yang baru saja dibuat pada folder `app\Models\Kendaraan.php`. Isikan dengan kode dibawah
    ```php
    <?php

    namespace App\Models;
    
    use Illuminate\Database\Eloquent\Model;
    
    class Kendaraan extends Model
    {
        protected $fillable = ['name', 'harga', 'gambar'];
    }

    ```

    Pada kode diatas, kita perlu menambahkan baris `protected $fillable = ['name', 'harga', 'gambar'];` agar kita dapat mengisi data dan menyimpan data ke database dengan Model yang dibuat.
4. Kembali ke file `app\Http\Controllers\KendaraanController.php`. Kita akan membuat kode baru untuk logika menambahkan data ke database dengan model `Kendaraan`. Buat fungsi baru dan beri nama `store`
   Jangan lupa, pastikan sudah import model `Kendaraan` kita dibaris atas pada controller. Kode lengkap sebagai berikut
   ```php
   // pastikan sudah ada kode untuk import model kendaraan
   // use App\Models\Kendaraan;
   // kode lain diatas
   public function store(Request $request)
    {
        // Validasi input
        $nama = $request->input('nama');
        $harga = $request->input('harga');

        // Handle file upload jika ada
        if ($request->hasFile('gambar')) {
            $imagePath = $request->file('gambar')->store('kendaraan', 'public');
            $validatedData['gambar'] = $imagePath;
        }

        // Simpan data kendaraan ke database
        Kendaraan::create(
            [
                'name' => $nama,
                'harga' => $harga,
                'gambar' => $imagePath,
            ]
        );

        return redirect()->route('admin.kendaraan.index')->with('success', 'Kendaraan berhasil ditambahkan.');
    }
   ```
5. Selanjutnya kita definisikan route dengan tipe `post` untuk mengarahkan request ke logika penambahan data ke database. Buka file `routes\web.php` tambahkan kode berikut
    ```php
    // kode lain diatas
    Route::post('/admin/kendaraan', [KendaraanController::class, 'store'])
      ->middleware('auth')
      ->name('admin.kendaraan.store');
    ```
6. Sebelum kita mencoba untuk menambahkan data baru, jalankan perintah untuk migrate database terlebih dahulu. Jalankan perintah berikut di git bash
    ```bash
    php artisan migrate
    ```
## Menampilkan data kendaraan dari database di Admin Panel
1. Buka kembali file `app\Http\Controllers\KendaraanController.php`, kita akan edit pada fungsi `index` yang sudah pernah dibuat sebelumnya. berikut kode lengkap pada fungsi index setelah diedit
    ```php
    public function index()
    {
        $kendaraan = Kendaraan::all();
        return view('admin.kendaraan', ['kendaraan' => $kendaraan]);
    }
    ```
2. Selanjutnya kita ubah kode pada file `resources\views\admin\kendaraan.blade.php` untuk menampilkan data kendaraan yang didapat dari database.
    Kode lengkap setelah diedit sebagai berikut
    ```html
    @extends('layouts.admin')
    @section('content')
        <main class="flex-1 p-6">
            <a href="{{ route('admin.kendaraan.create') }}" class="bg-purple-800 text-white px-2 py-1 mb-2 rounded inline-block">
                Tambah Kendaraan
            </a>
    
            <table class="w-full">
                <thead class="bg-gray-500 text-white">
                    <tr>
                        <th>
                            Gambar
                        </th>
                        <th>
                            Nama
                        </th>
                        <th>
                            Harga
                        </th>
                        <th>
                        </th>
                    </tr>
                </thead>
                <tbody>
                    @foreach ($kendaraan as $item)
                    <tr class="text-center">
                        <td>
                            <img src="{{ asset('storage/' . $item->gambar) }}" alt="{{ $item->name }}" class="w-20 mx-auto" />
                        </td>
                        <td>
                            {{ $item->name }}
                        </td>
                        <td>
                            {{ $item->harga }}
                        </td>
                        <td class="flex gap-1 justify-center">
                            <a href="{{ route('admin.kendaraan.edit', $item->id) }}" class="bg-purple-800 px-3 py-2 text-white mt-2">
                                Edit
                            </a>
                            <form action="{{ route('admin.kendaraan.destroy', $item->id) }}" method="POST" onsubmit="return confirm('Apakah anda yakin ingin menghapus data ini?');">
                                @csrf
                                @method('DELETE')
                                <button type="submit" class="bg-red-800 px-3 py-2 text-white mt-2">
                                    Hapus
                                </button>
                            </form>
                        </td>
                    @endforeach
                </tbody>
            </table>
        </main>
    @endsection
    ```
3. Terakhir, kita perlu menjalankan perintah `link` agar gambar yang kita upload dapat ditampilkan di `views`. Buka git bash dan jalankan perintah berikut
    ```bash
    php artisan storage:link
    ```

