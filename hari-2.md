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


### Penambahan kode baru di file `resources/views/welcome.blade.php`
```
{{-- feature section --}}
    <div class="grid grid-cols-3">
        <div class="text-center mt-2 space-y-2 p-4">
            <svg xmlns="http://www.w3.org/2000/svg" class="mx-auto size-10 " width="65" height="64"
                viewBox="0 0 65 64" fill="none">
                <g clip-path="url(#clip0_1_8291)">
                    <mask id="mask0_1_8291" style="mask-type:luminance" maskUnits="userSpaceOnUse" x="0" y="0"
                        width="65" height="64">
                        <path d="M0.5 7.62939e-06H64.5V64H0.5V7.62939e-06Z" fill="white" />
                    </mask>
                    <g mask="url(#mask0_1_8291)">
                        <path
                            d="M36.1384 43.6266C45.0582 44.1071 51.8006 46.322 51.8006 48.9817C51.8006 51.9927 43.1602 54.4336 32.5018 54.4336C21.8433 54.4336 13.2031 51.9927 13.2031 48.9817C13.2031 46.322 19.9453 44.1071 28.8651 43.6266"
                            stroke="black" stroke-width="4" stroke-miterlimit="10" stroke-linecap="round"
                            stroke-linejoin="round" />
                        <path
                            d="M6.86169 46.5148C4.01794 48.077 2.37494 49.9183 2.37494 51.8901C2.37494 57.5427 15.8624 62.125 32.4999 62.125C49.1376 62.125 62.6249 57.5427 62.6249 51.8901C62.6249 49.9183 60.9821 48.077 58.1383 46.5148"
                            stroke="black" stroke-width="4" stroke-miterlimit="10" stroke-linecap="round"
                            stroke-linejoin="round" />
                        <path
                            d="M32.5004 21.3638C29.6668 21.3638 27.3696 19.0667 27.3696 16.2332C27.3696 13.3995 29.6668 11.1024 32.5004 11.1024C35.334 11.1024 37.6311 13.3995 37.6311 16.2332C37.6311 19.0667 35.334 21.3638 32.5004 21.3638ZM32.5004 1.87491C23.9095 1.87491 16.9453 8.83904 16.9453 17.4297C16.9453 23.3948 25.6608 38.4044 30.0441 45.5762C31.1671 47.4134 33.8336 47.4134 34.9566 45.5762C39.34 38.4044 48.0555 23.3948 48.0555 17.4297C48.0555 8.83904 41.0913 1.87491 32.5004 1.87491Z"
                            stroke="black" stroke-width="4" stroke-miterlimit="10" stroke-linecap="round"
                            stroke-linejoin="round" />
                    </g>
                </g>
                <defs>
                    <clipPath id="clip0_1_8291">
                        <rect width="64" height="64" fill="white" transform="translate(0.5)" />
                    </clipPath>
                </defs>
            </svg>
            <h3 class="text-3xl font-bold">Mudah ditemukan</h3>
            <p>Temukan mobil yang Anda butuhkan kapan saja.</p>
        </div>
        <div class="text-center mt-2 space-y-2 p-4">
            <svg xmlns="http://www.w3.org/2000/svg" width="64" height="64" viewBox="0 0 64 64" fill="none"
                class="mx-auto size-10">
                <path d="M22.9609 43.0459H41.0362" stroke="black" stroke-width="4" stroke-miterlimit="10"
                    stroke-linecap="round" stroke-linejoin="round" />
                <mask id="mask0_1_8308" style="mask-type:luminance" maskUnits="userSpaceOnUse" x="0" y="0"
                    width="64" height="64">
                    <path d="M0 7.62939e-06H64V64H0V7.62939e-06Z" fill="white" />
                </mask>
                <g mask="url(#mask0_1_8308)">
                    <path
                        d="M53.0874 43.0459H57.104C59.8655 43.0459 62.125 40.7864 62.125 38.0251V37.0208C62.125 31.498 57.6061 26.9793 52.0832 26.9793H6.89575C4.13438 26.9793 1.875 29.2385 1.875 32V38.0251C1.875 40.7864 4.13438 43.0459 6.89575 43.0459H10.9129"
                        stroke="black" stroke-width="4" stroke-miterlimit="10" stroke-linecap="round"
                        stroke-linejoin="round" />
                    <path d="M22.9609 43.0459H41.0363" stroke="black" stroke-width="4" stroke-miterlimit="10"
                        stroke-linecap="round" stroke-linejoin="round" />
                    <path d="M29.9921 14.9292V26.9792" stroke="black" stroke-width="4" stroke-miterlimit="10"
                        stroke-linecap="round" stroke-linejoin="round" />
                    <path
                        d="M50.0729 26.9792L46.2931 19.4201C45.0585 16.9502 41.7885 14.9292 39.027 14.9292H20.9521C18.1906 14.9292 14.9208 16.9502 13.6861 19.4201L9.90625 26.9792"
                        stroke="black" stroke-width="4" stroke-miterlimit="10" stroke-linecap="round"
                        stroke-linejoin="round" />
                    <path
                        d="M53.0886 43.0459C53.0886 46.3733 50.3908 49.0708 47.0639 49.0708C43.7369 49.0708 41.0391 46.3733 41.0391 43.0459C41.0391 39.7183 43.7369 37.0208 47.0639 37.0208C50.3908 37.0208 53.0886 39.7183 53.0886 43.0459Z"
                        stroke="black" stroke-width="4" stroke-miterlimit="10" stroke-linecap="round"
                        stroke-linejoin="round" />
                    <path
                        d="M22.9637 43.0459C22.9637 46.3733 20.2659 49.0708 16.9391 49.0708C13.6121 49.0708 10.9141 46.3733 10.9141 43.0459C10.9141 39.7183 13.6121 37.0208 16.9391 37.0208C20.2659 37.0208 22.9637 39.7183 22.9637 43.0459Z"
                        stroke="black" stroke-width="4" stroke-miterlimit="10" stroke-linecap="round"
                        stroke-linejoin="round" />
                    <path d="M61.9188 35.0125H59.1094" stroke="black" stroke-width="4" stroke-miterlimit="10"
                        stroke-linecap="round" stroke-linejoin="round" />
                    <path d="M33.0004 35.0125H30.9922" stroke="black" stroke-width="4" stroke-miterlimit="10"
                        stroke-linecap="round" stroke-linejoin="round" />
                </g>
            </svg>
            <h3 class="text-3xl font-bold">Kenyamanan</h3>
            <p>Nikmati perjalanan Anda dengan mobil terbaik dan berkualitas.</p>
        </div>
        <div class="text-center mt-2 space-y-2 p-4">
            <svg xmlns="http://www.w3.org/2000/svg" width="65" height="64" viewBox="0 0 65 64"
                class="mx-auto size-10" fill="none">
                <g clip-path="url(#clip0_1_8337)">
                    <mask id="mask0_1_8337" style="mask-type:luminance" maskUnits="userSpaceOnUse" x="0" y="0"
                        width="65" height="64">
                        <path d="M0.5 7.62939e-06H64.5V64H0.5V7.62939e-06Z" fill="white" />
                    </mask>
                    <g mask="url(#mask0_1_8337)">
                        <path
                            d="M51.9922 16.9956V11.99C51.9922 9.23173 49.7561 6.99561 46.9978 6.99561H7.99219C5.23081 6.99561 2.99219 9.23423 2.99219 11.9956C2.99219 14.757 5.23081 16.9956 7.99219 16.9956H56.9978C59.7561 16.9956 61.9922 19.2317 61.9922 21.99V29.4956"
                            stroke="black" stroke-width="4" stroke-miterlimit="10" />
                        <path
                            d="M61.9922 44.4956V52.0012C61.9922 54.7595 59.7561 56.9956 56.9978 56.9956H7.99219C5.23081 56.9956 2.99219 54.7571 2.99219 51.9956V11.9956"
                            stroke="black" stroke-width="4" stroke-miterlimit="10" />
                        <path
                            d="M61.9922 44.4956H49.4922C45.3501 44.4956 41.9922 41.1377 41.9922 36.9956C41.9922 32.8535 45.3501 29.4956 49.4922 29.4956H61.9922V44.4956Z"
                            stroke="black" stroke-width="4" stroke-miterlimit="10" />
                    </g>
                </g>
                <defs>
                    <clipPath id="clip0_1_8337">
                        <rect width="64" height="64" fill="white" transform="translate(0.5)" />
                    </clipPath>
                </defs>
            </svg>
            <h3 class="text-3xl font-bold">Harga Bersahabat</h3>
            <p>Dapatkan penawaran terbaik untuk harga sewa mobil sesuai kebutuhan Anda.</p>
        </div>
    </div>
```
