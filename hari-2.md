## Catatan

### Menjalankan proyek laravel
- `php artisan serve` untuk menjalankan server php
- `npm run dev` untuk menjalankan developmnet server di nodejs/javascript

### file `resources/css/app.css`

```
@import 'tailwindcss';

@source '../../vendor/laravel/framework/src/Illuminate/Pagination/resources/views/*.blade.php';
@source '../../storage/framework/views/*.php';
@source '../**/*.blade.php';
@source '../**/*.js';

@theme {
    --font-sans: 'Instrument Sans', ui-sans-serif, system-ui, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji',
        'Segoe UI Symbol', 'Noto Color Emoji';
    --font-abel: 'Abel', sans-serif;
}

```
