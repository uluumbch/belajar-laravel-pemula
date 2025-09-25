### Catatan

- Membuat controller baru untuk admin
  ```bash
  php artisan make:controller AdminController
  ```
- Membuat halaman layout baru untuk admin
- Mengubah routes pada file `routes/web.php`
  ```php
  <?php

  use Illuminate\Support\Facades\Route;
  use App\Http\Controllers\LandingPageController;
  use App\Http\Controllers\AuthController;
  use App\Http\Controllers\AdminController;
  
  
  Route::get('/', [LandingPageController::class, 'home']);
  
  Route::get('/kendaraan', [LandingPageController::class, 'kendaraan']);
  
  Route::get('/login', [AuthController::class, 'loginPage'])->name('login');
  
  Route::post('/login', [AuthController::class, 'login']);
  
  Route::get('/admin', [AdminController::class, 'admin'])->middleware('auth');
  ```
