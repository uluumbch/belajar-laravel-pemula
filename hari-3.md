## Catatan

- `php artisan migrate` perintah untuk membuat database di laravel
- pastikan konfigurasi di file `.env` telah sesuai dengan database
  ```
  DB_CONNECTION=mysql
  DB_HOST=127.0.0.1
  DB_PORT=3306
  DB_DATABASE=rentalin
  DB_USERNAME=root
  DB_PASSWORD=
  ```

### Jalankan perintah berikut untuk menambahkan data user baru ke database
1. Buka terminal(git bash)
2. Jalankan perintah `php artisan tinker`
3. Shell tinker akan terbuka lalu jalankan perintah ini 1 per 1
   ```bash
   $user = new User();
   $user->name = "test";
   $user->email = "test@mail.com";
   $user->password = bcrypt("password");
   $user->save();
   ```  
4. untuk konfirmasi, cek database dengan phpmyadmin atau heidisql, pastikan terdapat data baru di table `users`


### Mengganti password user yg sudah terbuat
1. Buka terminal(git bash)
2. Jalankan perintah `php artisan tinker`
3. Shell tinker akan terbuka lalu jalankan perintah berikut
   Sesuaikan `test@mail.com` dengan email yang sudah ada dan `password` sesuai yg ingin diganti
   ```bash
   User::whereEmail('test@mail.com')->update(['password' => bcrypt('password')])
   ```
4. Contoh hasil dari perintah diatas sebagai berikut.
   ```bash
   [!] Aliasing 'User' to 'App\Models\User' for this Tinker session.
    = 1
   ```
