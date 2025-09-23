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
```blade
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

### Penambahan kode baru pada file `resources/views/welcome.blade.php` untuk membuat section mengapa memilih kami
```blade
{{-- memilih kami section --}}
    <div class="flex">

        <div class="w-1/2 pr-4">
            <img src="{{ asset('gambar/Gemini_Generated_Image_utpskjutpskjutps.png') }}"
                class="rounded-2xl object-cover" />
        </div>

        <div class="w-1/2 flex flex-col justify-center">
            <h2 class="text-3xl font-bold mb-4">
                Mengapa memilih kami?
            </h2>
            <ul class="space-y-6">
                <li class="space-y-2">
                    <span
                        class="inline-flex justify-center items-center bg-purple-800 text-white p-2 rounded-full h-8 w-8">1</span>
                    <span class="font-semibold">Armada terbaru & terawat</span>

                    <p>
                        Nikmati kenyamanan berkendara dengan pilihan mobil yang selalu bersih, terawat, dan siap
                        menemani
                        perjalanan Anda.
                    </p>
                </li>
                <li class="space-y-2">
                    <span
                        class="inline-flex justify-center items-center bg-purple-800 text-white p-2 rounded-full h-8 w-8">2</span>
                    <span class="font-semibold">Harga Transparan & Terjangkau</span>

                    <p>
                        Tanpa biaya tersembunyi, tanpa kejutan. Semua harga jelas sejak awal, sesuai dengan kebutuhan
                        Anda.
                    </p>
                </li>
                <li class="space-y-2">
                    <span
                        class="inline-flex justify-center items-center bg-purple-800 text-white p-2 rounded-full h-8 w-8">3</span>
                    <span class="font-semibold">Proses Cepat & Mudah</span>

                    <p>
                        Booking mobil dalam hitungan menit, tanpa ribet. Cukup pilih mobil, tentukan waktu, dan Anda siap berangkat!
                    </p>
                </li>
                <li class="space-y-2"> 
                    <span
                        class="inline-flex justify-center items-center bg-purple-800 text-white p-2 rounded-full h-8 w-8">4</span>
                    <span class="font-semibold">Layanan Pelanggan 24/7</span>

                    <p>
                        Tim kami siap membantu Anda kapan saja, di mana saja, agar perjalanan Anda tetap aman dan nyaman.
                    </p>
                </li>
                <li class="space-y-2">
                    <span
                        class="inline-flex justify-center items-center bg-purple-800 text-white p-2 rounded-full h-8 w-8">5</span>
                    <span class="font-semibold">Fleksibel untuk Semua Kebutuhan</span>

                    <p>
                        Mulai dari perjalanan bisnis, liburan keluarga, hingga kebutuhan harian — kami punya mobil yang tepat untuk Anda.
                    </p>
                </li>
            </ul>
        </div>

    </div>
```


### Penambahan kode baru di file `resources/views/welcome.blade.php` untuk membuat section pilihan mobil
```blade
{{-- pilihan mobil --}}
    <div class="mt-4">
        <div class="flex items-center justify-between  mx-6">
            <h2 class="font-semibold text-2xl">
               Pilih mobil yang cocok untuk kamu. 
            </h2>
            <a href="" class="text-purple-800 text-lg">
                Lihat semua
            </a>
        </div>

        <div class="grid grid-cols-3 gap-3">
            <div class="shadow-md">
                <img src="{{ asset('gambar/honda-brio.png') }}" class="h-52 w-2/3 object-cover mx-auto" />
                <div class="p-4">
                    <div class="flex justify-between">
                        <h3 class="font-semibold text-xl">
                            Honda Brio
                        </h3>
                        <p>
                            Rp125.000/hari
                        </p>
                    </div>
                </div>
                <a class="text-center block bg-purple-800 m-2 text-white rounded-lg py-2">
                    Sewa Sekarang
                </a>
            </div>
            <div class="shadow-md">
                <img src="{{ asset('gambar/honda-brio.png') }}" class="h-52 w-2/3 object-cover mx-auto" />
                <div class="p-4">
                    <div class="flex justify-between">
                        <h3 class="font-semibold text-xl">
                            Honda Brio
                        </h3>
                        <p>
                            Rp125.000/hari
                        </p>
                    </div>
                </div>
                <a class="text-center block bg-purple-800 m-2 text-white rounded-lg py-2">
                    Sewa Sekarang
                </a>
            </div>
            <div class="shadow-md">
                <img src="{{ asset('gambar/honda-brio.png') }}" class="h-52 w-2/3 object-cover mx-auto" />
                <div class="p-4">
                    <div class="flex justify-between">
                        <h3 class="font-semibold text-xl">
                            Honda Brio
                        </h3>
                        <p>
                            Rp125.000/hari
                        </p>
                    </div>
                </div>
                <a class="text-center block bg-purple-800 m-2 text-white rounded-lg py-2">
                    Sewa Sekarang
                </a>
            </div>
        </div>

    </div>
```

### Full COde untuk file `resources/views/welcome.blade.php`
```blade
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Rentalin</title>
    @vite('resources/css/app.css')
</head>

<body class="mx-6">
    <nav class="p-4 my-2 flex justify-between items-center">
        <div class="flex gap-x-2 items-center">
            <svg xmlns="http://www.w3.org/2000/svg" width="46" height="30" viewBox="0 0 46 30" fill="none">
                <path
                    d="M45.3383 16.8956C45.0008 13.1072 44.4448 12.3694 44.2348 12.0919C43.752 11.4506 42.9795 11.0316 42.162 10.5919C42.1158 10.5674 42.0759 10.5326 42.0454 10.4901C42.015 10.4476 41.9948 10.3985 41.9865 10.3469C41.9783 10.2953 41.9821 10.2424 41.9977 10.1925C42.0134 10.1426 42.0404 10.097 42.0767 10.0594C42.2281 9.90584 42.3445 9.72134 42.4178 9.51856C42.4911 9.31579 42.5196 9.09954 42.5014 8.88469C42.4661 8.5037 42.289 8.14987 42.0051 7.89339C41.7211 7.6369 41.3512 7.49649 40.9686 7.5H39.5061C39.4434 7.50037 39.3808 7.50444 39.3186 7.51219C39.2759 7.49367 39.2317 7.47893 39.1864 7.46813C38.3201 5.63719 37.1342 3.13031 34.6761 1.90687C31.0301 0.0937496 24.3139 0 23.0014 0C21.6889 0 14.9726 0.0937498 11.3314 1.90406C8.87327 3.1275 7.68733 5.63438 6.82108 7.46531L6.81358 7.48031C6.77038 7.48639 6.72795 7.49708 6.68702 7.51219C6.62481 7.50444 6.56221 7.50037 6.49952 7.5H5.03421C4.65161 7.49649 4.28166 7.6369 3.99774 7.89339C3.71381 8.14987 3.53665 8.5037 3.5014 8.88469C3.48474 9.09904 3.51457 9.31446 3.58884 9.51623C3.6631 9.71799 3.78006 9.90135 3.93171 10.0538C3.96799 10.0914 3.99502 10.137 4.01067 10.1869C4.02632 10.2368 4.03016 10.2896 4.02189 10.3413C4.01361 10.3929 3.99345 10.4419 3.963 10.4844C3.93254 10.527 3.89263 10.5618 3.8464 10.5863C3.0289 11.0287 2.25265 11.4478 1.77358 12.0863C1.56358 12.3675 1.00858 13.1016 0.670145 16.89C0.482645 19.0219 0.45452 21.2288 0.601707 22.65C0.910145 25.6031 1.48858 27.3881 1.51296 27.4622C1.60172 27.7317 1.76511 27.9705 1.98415 28.1509C2.2032 28.3313 2.46892 28.4458 2.75046 28.4812V28.5C2.75046 28.8978 2.90849 29.2794 3.1898 29.5607C3.4711 29.842 3.85263 30 4.25046 30H9.50046C9.89828 30 10.2798 29.842 10.5611 29.5607C10.8424 29.2794 11.0005 28.8978 11.0005 28.5C11.8076 28.5 12.3692 28.3556 12.9645 28.2019C13.824 27.9703 14.7025 27.8162 15.5895 27.7416C18.4498 27.4688 21.2942 27.375 23.0014 27.375C24.6739 27.375 27.6439 27.4688 30.5089 27.7416C31.3994 27.8164 32.2814 27.9711 33.1442 28.2038C33.7142 28.35 34.2551 28.485 35.0042 28.4991C35.0042 28.8969 35.1622 29.2784 35.4436 29.5597C35.7249 29.841 36.1064 29.9991 36.5042 29.9991H41.7542C42.152 29.9991 42.5336 29.841 42.8149 29.5597C43.0962 29.2784 43.2542 28.8969 43.2542 28.4991V28.4878C43.5364 28.4531 43.8029 28.3388 44.0227 28.1584C44.2425 27.978 44.4064 27.7388 44.4955 27.4688C44.5198 27.3947 45.0983 25.6097 45.4067 22.6566C45.5539 21.2344 45.5276 19.0312 45.3383 16.8956ZM9.53233 8.74781C10.2823 7.15406 11.1401 5.35031 12.6673 4.59C14.8742 3.49125 19.4483 2.99625 23.0014 2.99625C26.5545 2.99625 31.1286 3.4875 33.3355 4.59C34.8626 5.35031 35.7167 7.155 36.4705 8.74781L36.5642 8.95125C36.619 9.06707 36.6433 9.19499 36.6346 9.32284C36.6259 9.45068 36.5847 9.57417 36.5147 9.68153C36.4448 9.78889 36.3485 9.87654 36.2351 9.93612C36.1216 9.9957 35.9948 10.0252 35.8667 10.0219C32.7514 9.9375 26.1889 9.6675 23.0014 9.6675C19.8139 9.6675 13.2514 9.94406 10.1314 10.0284C10.0033 10.0318 9.87649 10.0023 9.76305 9.94268C9.64961 9.8831 9.55333 9.79545 9.48338 9.68809C9.41344 9.58073 9.37216 9.45724 9.3635 9.3294C9.35484 9.20156 9.37907 9.07363 9.4339 8.95781C9.46671 8.88844 9.5014 8.81812 9.53233 8.74781ZM10.6508 16.2131C9.03809 16.4072 7.41509 16.503 5.79077 16.5C4.79702 16.5 3.77233 16.2188 3.58202 15.3337C3.45171 14.7384 3.46577 14.4038 3.53608 14.0672C3.59514 13.7812 3.6889 13.5731 4.15765 13.5C5.3764 13.3125 6.05796 13.5478 8.05296 14.1356C9.37577 14.5247 10.3301 15.0431 10.8739 15.4537C11.1467 15.6562 11.0014 16.185 10.6508 16.2131ZM31.4051 23.9006C30.1714 24.0413 27.7039 23.9897 23.0295 23.9897C18.3551 23.9897 15.8886 24.0413 14.6548 23.9006C13.3817 23.7591 11.7589 22.5553 12.867 21.4828C13.6048 20.7759 15.3261 20.2472 17.6183 19.95C19.9105 19.6528 20.8808 19.5 23.0201 19.5C25.1595 19.5 26.0314 19.5938 28.422 19.9509C30.8126 20.3081 32.6192 20.8434 33.1733 21.4837C34.1839 22.6313 32.6773 23.7516 31.4051 23.9062V23.9006ZM42.4208 15.3328C42.2333 16.2216 41.202 16.4991 40.212 16.4991C38.5566 16.4994 36.9026 16.4037 35.2583 16.2122C34.9714 16.185 34.8383 15.6816 35.1289 15.4528C35.6642 15.0319 36.6289 14.5238 37.9498 14.1347C39.9448 13.5469 41.0951 13.3116 42.0833 13.5075C42.3242 13.5553 42.4517 13.8141 42.4667 13.9762C42.5328 14.4278 42.5173 14.8877 42.4208 15.3337V15.3328Z"
                    fill="black" />
            </svg>
            <h1 class="text-2xl ">Rentalin</h1>
        </div>
        {{-- links --}}
        <div class="space-x-2">
            <a href="">Beranda</a>
            <a href="">Kendaraan</a>
            <a href="">Tentang Kami</a>
        </div>

        {{-- contanct --}}
        <div>
            <p class="text-lg">Contact us</p>
            <span class="font-semibold">+62 812-3456-7890</span>
        </div>
    </nav>

    {{-- hero section --}}
    <div class="flex justify-between items-center bg-purple-800 mx-4 rounded-2xl">
        <div class="text-white p-5 max-w-xl">
            <h2 class="text-4xl font-bold">
                Temukan mobil impian Anda dengan mudah dan cepat
            </h2>
            <p class="mt-2">
                Platform terpercaya untuk sewa mobil di seluruh indonesia.
            </p>
            <button class="mt-2 px-4 py-3 rounded-lg bg-purple-400">
                Lihat Kendaraan
            </button>
        </div>
        <div>
            <img class="h-96" src="{{ asset('gambar/kijang-innova.png') }}" />
        </div>
    </div>

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

    {{-- memilih kami section --}}
    <div class="flex">

        <div class="w-1/2 pr-4">
            <img src="{{ asset('gambar/Gemini_Generated_Image_utpskjutpskjutps.png') }}"
                class="rounded-2xl object-cover" />
        </div>

        <div class="w-1/2 flex flex-col justify-center">
            <h2 class="text-3xl font-bold mb-4">
                Mengapa memilih kami?
            </h2>
            <ul class="space-y-6">
                <li class="space-y-2">
                    <span
                        class="inline-flex justify-center items-center bg-purple-800 text-white p-2 rounded-full h-8 w-8">1</span>
                    <span class="font-semibold">Armada terbaru & terawat</span>

                    <p>
                        Nikmati kenyamanan berkendara dengan pilihan mobil yang selalu bersih, terawat, dan siap
                        menemani
                        perjalanan Anda.
                    </p>
                </li>
                <li class="space-y-2">
                    <span
                        class="inline-flex justify-center items-center bg-purple-800 text-white p-2 rounded-full h-8 w-8">2</span>
                    <span class="font-semibold">Harga Transparan & Terjangkau</span>

                    <p>
                        Tanpa biaya tersembunyi, tanpa kejutan. Semua harga jelas sejak awal, sesuai dengan kebutuhan
                        Anda.
                    </p>
                </li>
                <li class="space-y-2">
                    <span
                        class="inline-flex justify-center items-center bg-purple-800 text-white p-2 rounded-full h-8 w-8">3</span>
                    <span class="font-semibold">Proses Cepat & Mudah</span>

                    <p>
                        Booking mobil dalam hitungan menit, tanpa ribet. Cukup pilih mobil, tentukan waktu, dan Anda
                        siap berangkat!
                    </p>
                </li>
                <li class="space-y-2">
                    <span
                        class="inline-flex justify-center items-center bg-purple-800 text-white p-2 rounded-full h-8 w-8">4</span>
                    <span class="font-semibold">Layanan Pelanggan 24/7</span>

                    <p>
                        Tim kami siap membantu Anda kapan saja, di mana saja, agar perjalanan Anda tetap aman dan
                        nyaman.
                    </p>
                </li>
                <li class="space-y-2">
                    <span
                        class="inline-flex justify-center items-center bg-purple-800 text-white p-2 rounded-full h-8 w-8">5</span>
                    <span class="font-semibold">Fleksibel untuk Semua Kebutuhan</span>

                    <p>
                        Mulai dari perjalanan bisnis, liburan keluarga, hingga kebutuhan harian — kami punya mobil yang
                        tepat untuk Anda.
                    </p>
                </li>
            </ul>
        </div>

    </div>

    {{-- pilihan mobil --}}
    <div class="mt-4">
        <div class="flex items-center justify-between  mx-6">
            <h2 class="font-semibold text-2xl">
                Pilih mobil yang cocok untuk kamu.
            </h2>
            <a href="" class="text-purple-800 text-lg">
                Lihat semua
            </a>
        </div>

        <div class="grid grid-cols-3 gap-3">
            <div class="shadow-md">
                <img src="{{ asset('gambar/honda-brio.png') }}" class="h-52 w-2/3 object-cover mx-auto" />
                <div class="p-4">
                    <div class="flex justify-between">
                        <h3 class="font-semibold text-xl">
                            Honda Brio
                        </h3>
                        <p>
                            Rp125.000/hari
                        </p>
                    </div>
                </div>
                <a class="text-center block bg-purple-800 m-2 text-white rounded-lg py-2">
                    Sewa Sekarang
                </a>
            </div>
            <div class="shadow-md">
                <img src="{{ asset('gambar/honda-brio.png') }}" class="h-52 w-2/3 object-cover mx-auto" />
                <div class="p-4">
                    <div class="flex justify-between">
                        <h3 class="font-semibold text-xl">
                            Honda Brio
                        </h3>
                        <p>
                            Rp125.000/hari
                        </p>
                    </div>
                </div>
                <a class="text-center block bg-purple-800 m-2 text-white rounded-lg py-2">
                    Sewa Sekarang
                </a>
            </div>
            <div class="shadow-md">
                <img src="{{ asset('gambar/honda-brio.png') }}" class="h-52 w-2/3 object-cover mx-auto" />
                <div class="p-4">
                    <div class="flex justify-between">
                        <h3 class="font-semibold text-xl">
                            Honda Brio
                        </h3>
                        <p>
                            Rp125.000/hari
                        </p>
                    </div>
                </div>
                <a class="text-center block bg-purple-800 m-2 text-white rounded-lg py-2">
                    Sewa Sekarang
                </a>
            </div>
        </div>

    </div>

    <footer class="flex justify-between my-4 items-center">

        <div>
            <div class="flex gap-x-2 items-center">
                <svg xmlns="http://www.w3.org/2000/svg" width="46" height="30" viewBox="0 0 46 30"
                    fill="none">
                    <path
                        d="M45.3383 16.8956C45.0008 13.1072 44.4448 12.3694 44.2348 12.0919C43.752 11.4506 42.9795 11.0316 42.162 10.5919C42.1158 10.5674 42.0759 10.5326 42.0454 10.4901C42.015 10.4476 41.9948 10.3985 41.9865 10.3469C41.9783 10.2953 41.9821 10.2424 41.9977 10.1925C42.0134 10.1426 42.0404 10.097 42.0767 10.0594C42.2281 9.90584 42.3445 9.72134 42.4178 9.51856C42.4911 9.31579 42.5196 9.09954 42.5014 8.88469C42.4661 8.5037 42.289 8.14987 42.0051 7.89339C41.7211 7.6369 41.3512 7.49649 40.9686 7.5H39.5061C39.4434 7.50037 39.3808 7.50444 39.3186 7.51219C39.2759 7.49367 39.2317 7.47893 39.1864 7.46813C38.3201 5.63719 37.1342 3.13031 34.6761 1.90687C31.0301 0.0937496 24.3139 0 23.0014 0C21.6889 0 14.9726 0.0937498 11.3314 1.90406C8.87327 3.1275 7.68733 5.63438 6.82108 7.46531L6.81358 7.48031C6.77038 7.48639 6.72795 7.49708 6.68702 7.51219C6.62481 7.50444 6.56221 7.50037 6.49952 7.5H5.03421C4.65161 7.49649 4.28166 7.6369 3.99774 7.89339C3.71381 8.14987 3.53665 8.5037 3.5014 8.88469C3.48474 9.09904 3.51457 9.31446 3.58884 9.51623C3.6631 9.71799 3.78006 9.90135 3.93171 10.0538C3.96799 10.0914 3.99502 10.137 4.01067 10.1869C4.02632 10.2368 4.03016 10.2896 4.02189 10.3413C4.01361 10.3929 3.99345 10.4419 3.963 10.4844C3.93254 10.527 3.89263 10.5618 3.8464 10.5863C3.0289 11.0287 2.25265 11.4478 1.77358 12.0863C1.56358 12.3675 1.00858 13.1016 0.670145 16.89C0.482645 19.0219 0.45452 21.2288 0.601707 22.65C0.910145 25.6031 1.48858 27.3881 1.51296 27.4622C1.60172 27.7317 1.76511 27.9705 1.98415 28.1509C2.2032 28.3313 2.46892 28.4458 2.75046 28.4812V28.5C2.75046 28.8978 2.90849 29.2794 3.1898 29.5607C3.4711 29.842 3.85263 30 4.25046 30H9.50046C9.89828 30 10.2798 29.842 10.5611 29.5607C10.8424 29.2794 11.0005 28.8978 11.0005 28.5C11.8076 28.5 12.3692 28.3556 12.9645 28.2019C13.824 27.9703 14.7025 27.8162 15.5895 27.7416C18.4498 27.4688 21.2942 27.375 23.0014 27.375C24.6739 27.375 27.6439 27.4688 30.5089 27.7416C31.3994 27.8164 32.2814 27.9711 33.1442 28.2038C33.7142 28.35 34.2551 28.485 35.0042 28.4991C35.0042 28.8969 35.1622 29.2784 35.4436 29.5597C35.7249 29.841 36.1064 29.9991 36.5042 29.9991H41.7542C42.152 29.9991 42.5336 29.841 42.8149 29.5597C43.0962 29.2784 43.2542 28.8969 43.2542 28.4991V28.4878C43.5364 28.4531 43.8029 28.3388 44.0227 28.1584C44.2425 27.978 44.4064 27.7388 44.4955 27.4688C44.5198 27.3947 45.0983 25.6097 45.4067 22.6566C45.5539 21.2344 45.5276 19.0312 45.3383 16.8956ZM9.53233 8.74781C10.2823 7.15406 11.1401 5.35031 12.6673 4.59C14.8742 3.49125 19.4483 2.99625 23.0014 2.99625C26.5545 2.99625 31.1286 3.4875 33.3355 4.59C34.8626 5.35031 35.7167 7.155 36.4705 8.74781L36.5642 8.95125C36.619 9.06707 36.6433 9.19499 36.6346 9.32284C36.6259 9.45068 36.5847 9.57417 36.5147 9.68153C36.4448 9.78889 36.3485 9.87654 36.2351 9.93612C36.1216 9.9957 35.9948 10.0252 35.8667 10.0219C32.7514 9.9375 26.1889 9.6675 23.0014 9.6675C19.8139 9.6675 13.2514 9.94406 10.1314 10.0284C10.0033 10.0318 9.87649 10.0023 9.76305 9.94268C9.64961 9.8831 9.55333 9.79545 9.48338 9.68809C9.41344 9.58073 9.37216 9.45724 9.3635 9.3294C9.35484 9.20156 9.37907 9.07363 9.4339 8.95781C9.46671 8.88844 9.5014 8.81812 9.53233 8.74781ZM10.6508 16.2131C9.03809 16.4072 7.41509 16.503 5.79077 16.5C4.79702 16.5 3.77233 16.2188 3.58202 15.3337C3.45171 14.7384 3.46577 14.4038 3.53608 14.0672C3.59514 13.7812 3.6889 13.5731 4.15765 13.5C5.3764 13.3125 6.05796 13.5478 8.05296 14.1356C9.37577 14.5247 10.3301 15.0431 10.8739 15.4537C11.1467 15.6562 11.0014 16.185 10.6508 16.2131ZM31.4051 23.9006C30.1714 24.0413 27.7039 23.9897 23.0295 23.9897C18.3551 23.9897 15.8886 24.0413 14.6548 23.9006C13.3817 23.7591 11.7589 22.5553 12.867 21.4828C13.6048 20.7759 15.3261 20.2472 17.6183 19.95C19.9105 19.6528 20.8808 19.5 23.0201 19.5C25.1595 19.5 26.0314 19.5938 28.422 19.9509C30.8126 20.3081 32.6192 20.8434 33.1733 21.4837C34.1839 22.6313 32.6773 23.7516 31.4051 23.9062V23.9006ZM42.4208 15.3328C42.2333 16.2216 41.202 16.4991 40.212 16.4991C38.5566 16.4994 36.9026 16.4037 35.2583 16.2122C34.9714 16.185 34.8383 15.6816 35.1289 15.4528C35.6642 15.0319 36.6289 14.5238 37.9498 14.1347C39.9448 13.5469 41.0951 13.3116 42.0833 13.5075C42.3242 13.5553 42.4517 13.8141 42.4667 13.9762C42.5328 14.4278 42.5173 14.8877 42.4208 15.3337V15.3328Z"
                        fill="black" />
                </svg>
                <h1 class="text-2xl ">Rentalin</h1>
            </div>
            <span>
                &copy; {{ date('Y') }}
            </span>
        </div>

        <div class="flex flex-col">
            <a href="">Beranda</a>
            <a href="">Kendaraan</a>
            <a href="">Tentang Kami</a>
        </div>
    </footer>

</body>

</html>
```
### Folder baru bernama `layouts` di `resources/views`
### File baru untuk layout `resources\views\layouts\app.blade.php`
```blade
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Rentalin</title>
    @vite('resources/css/app.css')
</head>

<body class="mx-6">
    <nav class="p-4 my-2 flex justify-between items-center">
        <div class="flex gap-x-2 items-center">
            <svg xmlns="http://www.w3.org/2000/svg" width="46" height="30" viewBox="0 0 46 30" fill="none">
                <path
                    d="M45.3383 16.8956C45.0008 13.1072 44.4448 12.3694 44.2348 12.0919C43.752 11.4506 42.9795 11.0316 42.162 10.5919C42.1158 10.5674 42.0759 10.5326 42.0454 10.4901C42.015 10.4476 41.9948 10.3985 41.9865 10.3469C41.9783 10.2953 41.9821 10.2424 41.9977 10.1925C42.0134 10.1426 42.0404 10.097 42.0767 10.0594C42.2281 9.90584 42.3445 9.72134 42.4178 9.51856C42.4911 9.31579 42.5196 9.09954 42.5014 8.88469C42.4661 8.5037 42.289 8.14987 42.0051 7.89339C41.7211 7.6369 41.3512 7.49649 40.9686 7.5H39.5061C39.4434 7.50037 39.3808 7.50444 39.3186 7.51219C39.2759 7.49367 39.2317 7.47893 39.1864 7.46813C38.3201 5.63719 37.1342 3.13031 34.6761 1.90687C31.0301 0.0937496 24.3139 0 23.0014 0C21.6889 0 14.9726 0.0937498 11.3314 1.90406C8.87327 3.1275 7.68733 5.63438 6.82108 7.46531L6.81358 7.48031C6.77038 7.48639 6.72795 7.49708 6.68702 7.51219C6.62481 7.50444 6.56221 7.50037 6.49952 7.5H5.03421C4.65161 7.49649 4.28166 7.6369 3.99774 7.89339C3.71381 8.14987 3.53665 8.5037 3.5014 8.88469C3.48474 9.09904 3.51457 9.31446 3.58884 9.51623C3.6631 9.71799 3.78006 9.90135 3.93171 10.0538C3.96799 10.0914 3.99502 10.137 4.01067 10.1869C4.02632 10.2368 4.03016 10.2896 4.02189 10.3413C4.01361 10.3929 3.99345 10.4419 3.963 10.4844C3.93254 10.527 3.89263 10.5618 3.8464 10.5863C3.0289 11.0287 2.25265 11.4478 1.77358 12.0863C1.56358 12.3675 1.00858 13.1016 0.670145 16.89C0.482645 19.0219 0.45452 21.2288 0.601707 22.65C0.910145 25.6031 1.48858 27.3881 1.51296 27.4622C1.60172 27.7317 1.76511 27.9705 1.98415 28.1509C2.2032 28.3313 2.46892 28.4458 2.75046 28.4812V28.5C2.75046 28.8978 2.90849 29.2794 3.1898 29.5607C3.4711 29.842 3.85263 30 4.25046 30H9.50046C9.89828 30 10.2798 29.842 10.5611 29.5607C10.8424 29.2794 11.0005 28.8978 11.0005 28.5C11.8076 28.5 12.3692 28.3556 12.9645 28.2019C13.824 27.9703 14.7025 27.8162 15.5895 27.7416C18.4498 27.4688 21.2942 27.375 23.0014 27.375C24.6739 27.375 27.6439 27.4688 30.5089 27.7416C31.3994 27.8164 32.2814 27.9711 33.1442 28.2038C33.7142 28.35 34.2551 28.485 35.0042 28.4991C35.0042 28.8969 35.1622 29.2784 35.4436 29.5597C35.7249 29.841 36.1064 29.9991 36.5042 29.9991H41.7542C42.152 29.9991 42.5336 29.841 42.8149 29.5597C43.0962 29.2784 43.2542 28.8969 43.2542 28.4991V28.4878C43.5364 28.4531 43.8029 28.3388 44.0227 28.1584C44.2425 27.978 44.4064 27.7388 44.4955 27.4688C44.5198 27.3947 45.0983 25.6097 45.4067 22.6566C45.5539 21.2344 45.5276 19.0312 45.3383 16.8956ZM9.53233 8.74781C10.2823 7.15406 11.1401 5.35031 12.6673 4.59C14.8742 3.49125 19.4483 2.99625 23.0014 2.99625C26.5545 2.99625 31.1286 3.4875 33.3355 4.59C34.8626 5.35031 35.7167 7.155 36.4705 8.74781L36.5642 8.95125C36.619 9.06707 36.6433 9.19499 36.6346 9.32284C36.6259 9.45068 36.5847 9.57417 36.5147 9.68153C36.4448 9.78889 36.3485 9.87654 36.2351 9.93612C36.1216 9.9957 35.9948 10.0252 35.8667 10.0219C32.7514 9.9375 26.1889 9.6675 23.0014 9.6675C19.8139 9.6675 13.2514 9.94406 10.1314 10.0284C10.0033 10.0318 9.87649 10.0023 9.76305 9.94268C9.64961 9.8831 9.55333 9.79545 9.48338 9.68809C9.41344 9.58073 9.37216 9.45724 9.3635 9.3294C9.35484 9.20156 9.37907 9.07363 9.4339 8.95781C9.46671 8.88844 9.5014 8.81812 9.53233 8.74781ZM10.6508 16.2131C9.03809 16.4072 7.41509 16.503 5.79077 16.5C4.79702 16.5 3.77233 16.2188 3.58202 15.3337C3.45171 14.7384 3.46577 14.4038 3.53608 14.0672C3.59514 13.7812 3.6889 13.5731 4.15765 13.5C5.3764 13.3125 6.05796 13.5478 8.05296 14.1356C9.37577 14.5247 10.3301 15.0431 10.8739 15.4537C11.1467 15.6562 11.0014 16.185 10.6508 16.2131ZM31.4051 23.9006C30.1714 24.0413 27.7039 23.9897 23.0295 23.9897C18.3551 23.9897 15.8886 24.0413 14.6548 23.9006C13.3817 23.7591 11.7589 22.5553 12.867 21.4828C13.6048 20.7759 15.3261 20.2472 17.6183 19.95C19.9105 19.6528 20.8808 19.5 23.0201 19.5C25.1595 19.5 26.0314 19.5938 28.422 19.9509C30.8126 20.3081 32.6192 20.8434 33.1733 21.4837C34.1839 22.6313 32.6773 23.7516 31.4051 23.9062V23.9006ZM42.4208 15.3328C42.2333 16.2216 41.202 16.4991 40.212 16.4991C38.5566 16.4994 36.9026 16.4037 35.2583 16.2122C34.9714 16.185 34.8383 15.6816 35.1289 15.4528C35.6642 15.0319 36.6289 14.5238 37.9498 14.1347C39.9448 13.5469 41.0951 13.3116 42.0833 13.5075C42.3242 13.5553 42.4517 13.8141 42.4667 13.9762C42.5328 14.4278 42.5173 14.8877 42.4208 15.3337V15.3328Z"
                    fill="black" />
            </svg>
            <h1 class="text-2xl ">Rentalin</h1>
        </div>
        {{-- links --}}
        <div class="space-x-2">
            <a href="">Beranda</a>
            <a class="text-black decoration-0" href="{{ url('/kendaraan') }}">Kendaraan</a>
            <a href="">Tentang Kami</a>
        </div>

        {{-- contanct --}}
        <div>
            <p class="text-lg">Contact us</p>
            <span class="font-semibold">+62 812-3456-7890</span>
        </div>
    </nav>
    @yield('content')

    <footer class="flex justify-between my-4 items-center">

        <div>
            <div class="flex gap-x-2 items-center">
                <svg xmlns="http://www.w3.org/2000/svg" width="46" height="30" viewBox="0 0 46 30"
                    fill="none">
                    <path
                        d="M45.3383 16.8956C45.0008 13.1072 44.4448 12.3694 44.2348 12.0919C43.752 11.4506 42.9795 11.0316 42.162 10.5919C42.1158 10.5674 42.0759 10.5326 42.0454 10.4901C42.015 10.4476 41.9948 10.3985 41.9865 10.3469C41.9783 10.2953 41.9821 10.2424 41.9977 10.1925C42.0134 10.1426 42.0404 10.097 42.0767 10.0594C42.2281 9.90584 42.3445 9.72134 42.4178 9.51856C42.4911 9.31579 42.5196 9.09954 42.5014 8.88469C42.4661 8.5037 42.289 8.14987 42.0051 7.89339C41.7211 7.6369 41.3512 7.49649 40.9686 7.5H39.5061C39.4434 7.50037 39.3808 7.50444 39.3186 7.51219C39.2759 7.49367 39.2317 7.47893 39.1864 7.46813C38.3201 5.63719 37.1342 3.13031 34.6761 1.90687C31.0301 0.0937496 24.3139 0 23.0014 0C21.6889 0 14.9726 0.0937498 11.3314 1.90406C8.87327 3.1275 7.68733 5.63438 6.82108 7.46531L6.81358 7.48031C6.77038 7.48639 6.72795 7.49708 6.68702 7.51219C6.62481 7.50444 6.56221 7.50037 6.49952 7.5H5.03421C4.65161 7.49649 4.28166 7.6369 3.99774 7.89339C3.71381 8.14987 3.53665 8.5037 3.5014 8.88469C3.48474 9.09904 3.51457 9.31446 3.58884 9.51623C3.6631 9.71799 3.78006 9.90135 3.93171 10.0538C3.96799 10.0914 3.99502 10.137 4.01067 10.1869C4.02632 10.2368 4.03016 10.2896 4.02189 10.3413C4.01361 10.3929 3.99345 10.4419 3.963 10.4844C3.93254 10.527 3.89263 10.5618 3.8464 10.5863C3.0289 11.0287 2.25265 11.4478 1.77358 12.0863C1.56358 12.3675 1.00858 13.1016 0.670145 16.89C0.482645 19.0219 0.45452 21.2288 0.601707 22.65C0.910145 25.6031 1.48858 27.3881 1.51296 27.4622C1.60172 27.7317 1.76511 27.9705 1.98415 28.1509C2.2032 28.3313 2.46892 28.4458 2.75046 28.4812V28.5C2.75046 28.8978 2.90849 29.2794 3.1898 29.5607C3.4711 29.842 3.85263 30 4.25046 30H9.50046C9.89828 30 10.2798 29.842 10.5611 29.5607C10.8424 29.2794 11.0005 28.8978 11.0005 28.5C11.8076 28.5 12.3692 28.3556 12.9645 28.2019C13.824 27.9703 14.7025 27.8162 15.5895 27.7416C18.4498 27.4688 21.2942 27.375 23.0014 27.375C24.6739 27.375 27.6439 27.4688 30.5089 27.7416C31.3994 27.8164 32.2814 27.9711 33.1442 28.2038C33.7142 28.35 34.2551 28.485 35.0042 28.4991C35.0042 28.8969 35.1622 29.2784 35.4436 29.5597C35.7249 29.841 36.1064 29.9991 36.5042 29.9991H41.7542C42.152 29.9991 42.5336 29.841 42.8149 29.5597C43.0962 29.2784 43.2542 28.8969 43.2542 28.4991V28.4878C43.5364 28.4531 43.8029 28.3388 44.0227 28.1584C44.2425 27.978 44.4064 27.7388 44.4955 27.4688C44.5198 27.3947 45.0983 25.6097 45.4067 22.6566C45.5539 21.2344 45.5276 19.0312 45.3383 16.8956ZM9.53233 8.74781C10.2823 7.15406 11.1401 5.35031 12.6673 4.59C14.8742 3.49125 19.4483 2.99625 23.0014 2.99625C26.5545 2.99625 31.1286 3.4875 33.3355 4.59C34.8626 5.35031 35.7167 7.155 36.4705 8.74781L36.5642 8.95125C36.619 9.06707 36.6433 9.19499 36.6346 9.32284C36.6259 9.45068 36.5847 9.57417 36.5147 9.68153C36.4448 9.78889 36.3485 9.87654 36.2351 9.93612C36.1216 9.9957 35.9948 10.0252 35.8667 10.0219C32.7514 9.9375 26.1889 9.6675 23.0014 9.6675C19.8139 9.6675 13.2514 9.94406 10.1314 10.0284C10.0033 10.0318 9.87649 10.0023 9.76305 9.94268C9.64961 9.8831 9.55333 9.79545 9.48338 9.68809C9.41344 9.58073 9.37216 9.45724 9.3635 9.3294C9.35484 9.20156 9.37907 9.07363 9.4339 8.95781C9.46671 8.88844 9.5014 8.81812 9.53233 8.74781ZM10.6508 16.2131C9.03809 16.4072 7.41509 16.503 5.79077 16.5C4.79702 16.5 3.77233 16.2188 3.58202 15.3337C3.45171 14.7384 3.46577 14.4038 3.53608 14.0672C3.59514 13.7812 3.6889 13.5731 4.15765 13.5C5.3764 13.3125 6.05796 13.5478 8.05296 14.1356C9.37577 14.5247 10.3301 15.0431 10.8739 15.4537C11.1467 15.6562 11.0014 16.185 10.6508 16.2131ZM31.4051 23.9006C30.1714 24.0413 27.7039 23.9897 23.0295 23.9897C18.3551 23.9897 15.8886 24.0413 14.6548 23.9006C13.3817 23.7591 11.7589 22.5553 12.867 21.4828C13.6048 20.7759 15.3261 20.2472 17.6183 19.95C19.9105 19.6528 20.8808 19.5 23.0201 19.5C25.1595 19.5 26.0314 19.5938 28.422 19.9509C30.8126 20.3081 32.6192 20.8434 33.1733 21.4837C34.1839 22.6313 32.6773 23.7516 31.4051 23.9062V23.9006ZM42.4208 15.3328C42.2333 16.2216 41.202 16.4991 40.212 16.4991C38.5566 16.4994 36.9026 16.4037 35.2583 16.2122C34.9714 16.185 34.8383 15.6816 35.1289 15.4528C35.6642 15.0319 36.6289 14.5238 37.9498 14.1347C39.9448 13.5469 41.0951 13.3116 42.0833 13.5075C42.3242 13.5553 42.4517 13.8141 42.4667 13.9762C42.5328 14.4278 42.5173 14.8877 42.4208 15.3337V15.3328Z"
                        fill="black" />
                </svg>
                <h1 class="text-2xl ">Rentalin</h1>
            </div>
            <span>
                &copy; {{ date('Y') }}
            </span>
        </div>

        <div class="flex flex-col">
            <a href="">Beranda</a>
            <a href="{{ url('/kendaraan') }}">Kendaraan</a>
            <a href="">Tentang Kami</a>
        </div>
    </footer>

</body>

</html>
```

### Update file `resources\views\welcome.blade.php`
```blade
@extends('layouts.app')
@section('content')
    {{-- hero section --}}
    <div class="flex justify-between items-center bg-purple-800 mx-4 rounded-2xl">
        <div class="text-white p-5 max-w-xl space-y-4">
            <h2 class="text-4xl font-bold">
                Temukan mobil impian Anda dengan mudah dan cepat
            </h2>
            <p class="mt-2">
                Platform terpercaya untuk sewa mobil di seluruh indonesia.
            </p>
            <a href="#kendaraan" class="px-4 py-3 rounded-lg bg-purple-400">
                Lihat Kendaraan
            </a>
        </div>

        <div>
            <img class="h-96" src="{{ asset('gambar/kijang-innova.png') }}" />
        </div>
    </div>

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
                <mask id="mask0_1_8308" style="mask-type:luminance" maskUnits="userSpaceOnUse" x="0" y="0" width="64"
                    height="64">
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

    {{-- memilih kami section --}}
    <div class="flex">

        <div class="w-1/2 pr-4">
            <img src="{{ asset('gambar/Gemini_Generated_Image_utpskjutpskjutps.png') }}"
                class="rounded-2xl object-cover" />
        </div>

        <div class="w-1/2 flex flex-col justify-center">
            <h2 class="text-3xl font-bold mb-4">
                Mengapa memilih kami?
            </h2>
            <ul class="space-y-6">
                <li class="space-y-2">
                    <span
                        class="inline-flex justify-center items-center bg-purple-800 text-white p-2 rounded-full h-8 w-8">1</span>
                    <span class="font-semibold">Armada terbaru & terawat</span>

                    <p>
                        Nikmati kenyamanan berkendara dengan pilihan mobil yang selalu bersih, terawat, dan siap
                        menemani
                        perjalanan Anda.
                    </p>
                </li>
                <li class="space-y-2">
                    <span
                        class="inline-flex justify-center items-center bg-purple-800 text-white p-2 rounded-full h-8 w-8">2</span>
                    <span class="font-semibold">Harga Transparan & Terjangkau</span>

                    <p>
                        Tanpa biaya tersembunyi, tanpa kejutan. Semua harga jelas sejak awal, sesuai dengan kebutuhan
                        Anda.
                    </p>
                </li>
                <li class="space-y-2">
                    <span
                        class="inline-flex justify-center items-center bg-purple-800 text-white p-2 rounded-full h-8 w-8">3</span>
                    <span class="font-semibold">Proses Cepat & Mudah</span>

                    <p>
                        Booking mobil dalam hitungan menit, tanpa ribet. Cukup pilih mobil, tentukan waktu, dan Anda
                        siap berangkat!
                    </p>
                </li>
                <li class="space-y-2">
                    <span
                        class="inline-flex justify-center items-center bg-purple-800 text-white p-2 rounded-full h-8 w-8">4</span>
                    <span class="font-semibold">Layanan Pelanggan 24/7</span>

                    <p>
                        Tim kami siap membantu Anda kapan saja, di mana saja, agar perjalanan Anda tetap aman dan
                        nyaman.
                    </p>
                </li>
                <li class="space-y-2">
                    <span
                        class="inline-flex justify-center items-center bg-purple-800 text-white p-2 rounded-full h-8 w-8">5</span>
                    <span class="font-semibold">Fleksibel untuk Semua Kebutuhan</span>

                    <p>
                        Mulai dari perjalanan bisnis, liburan keluarga, hingga kebutuhan harian — kami punya mobil yang
                        tepat untuk Anda.
                    </p>
                </li>
            </ul>
        </div>

    </div>

    {{-- pilihan mobil --}}
    <div id="kendaraan" class="mt-4">
        <div class="flex items-center justify-between  mx-6">
            <h2 class="font-semibold text-2xl">
                Pilih mobil yang cocok untuk kamu.
            </h2>
            <a href="" class="text-purple-800 text-lg">
                Lihat semua
            </a>
        </div>

        <div class="grid grid-cols-3 gap-3">
            <div class="shadow-md">
                <img src="{{ asset('gambar/honda-brio.png') }}" class="h-52 w-2/3 object-cover mx-auto" />
                <div class="p-4">
                    <div class="flex justify-between">
                        <h3 class="font-semibold text-xl">
                            Honda Brio
                        </h3>
                        <p>
                            Rp125.000/hari
                        </p>
                    </div>
                </div>
                <a class="text-center block bg-purple-800 m-2 text-white rounded-lg py-2">
                    Sewa Sekarang
                </a>
            </div>
            <div class="shadow-md">
                <img src="{{ asset('gambar/honda-brio.png') }}" class="h-52 w-2/3 object-cover mx-auto" />
                <div class="p-4">
                    <div class="flex justify-between">
                        <h3 class="font-semibold text-xl">
                            Honda Brio
                        </h3>
                        <p>
                            Rp125.000/hari
                        </p>
                    </div>
                </div>
                <a class="text-center block bg-purple-800 m-2 text-white rounded-lg py-2">
                    Sewa Sekarang
                </a>
            </div>
            <div class="shadow-md">
                <img src="{{ asset('gambar/honda-brio.png') }}" class="h-52 w-2/3 object-cover mx-auto" />
                <div class="p-4">
                    <div class="flex justify-between">
                        <h3 class="font-semibold text-xl">
                            Honda Brio
                        </h3>
                        <p>
                            Rp125.000/hari
                        </p>
                    </div>
                </div>
                <a class="text-center block bg-purple-800 m-2 text-white rounded-lg py-2">
                    Sewa Sekarang
                </a>
            </div>
        </div>

    </div>

    <footer class="flex justify-between my-4 items-center">

        <div>
            <div class="flex gap-x-2 items-center">
                <svg xmlns="http://www.w3.org/2000/svg" width="46" height="30" viewBox="0 0 46 30"
                    fill="none">
                    <path
                        d="M45.3383 16.8956C45.0008 13.1072 44.4448 12.3694 44.2348 12.0919C43.752 11.4506 42.9795 11.0316 42.162 10.5919C42.1158 10.5674 42.0759 10.5326 42.0454 10.4901C42.015 10.4476 41.9948 10.3985 41.9865 10.3469C41.9783 10.2953 41.9821 10.2424 41.9977 10.1925C42.0134 10.1426 42.0404 10.097 42.0767 10.0594C42.2281 9.90584 42.3445 9.72134 42.4178 9.51856C42.4911 9.31579 42.5196 9.09954 42.5014 8.88469C42.4661 8.5037 42.289 8.14987 42.0051 7.89339C41.7211 7.6369 41.3512 7.49649 40.9686 7.5H39.5061C39.4434 7.50037 39.3808 7.50444 39.3186 7.51219C39.2759 7.49367 39.2317 7.47893 39.1864 7.46813C38.3201 5.63719 37.1342 3.13031 34.6761 1.90687C31.0301 0.0937496 24.3139 0 23.0014 0C21.6889 0 14.9726 0.0937498 11.3314 1.90406C8.87327 3.1275 7.68733 5.63438 6.82108 7.46531L6.81358 7.48031C6.77038 7.48639 6.72795 7.49708 6.68702 7.51219C6.62481 7.50444 6.56221 7.50037 6.49952 7.5H5.03421C4.65161 7.49649 4.28166 7.6369 3.99774 7.89339C3.71381 8.14987 3.53665 8.5037 3.5014 8.88469C3.48474 9.09904 3.51457 9.31446 3.58884 9.51623C3.6631 9.71799 3.78006 9.90135 3.93171 10.0538C3.96799 10.0914 3.99502 10.137 4.01067 10.1869C4.02632 10.2368 4.03016 10.2896 4.02189 10.3413C4.01361 10.3929 3.99345 10.4419 3.963 10.4844C3.93254 10.527 3.89263 10.5618 3.8464 10.5863C3.0289 11.0287 2.25265 11.4478 1.77358 12.0863C1.56358 12.3675 1.00858 13.1016 0.670145 16.89C0.482645 19.0219 0.45452 21.2288 0.601707 22.65C0.910145 25.6031 1.48858 27.3881 1.51296 27.4622C1.60172 27.7317 1.76511 27.9705 1.98415 28.1509C2.2032 28.3313 2.46892 28.4458 2.75046 28.4812V28.5C2.75046 28.8978 2.90849 29.2794 3.1898 29.5607C3.4711 29.842 3.85263 30 4.25046 30H9.50046C9.89828 30 10.2798 29.842 10.5611 29.5607C10.8424 29.2794 11.0005 28.8978 11.0005 28.5C11.8076 28.5 12.3692 28.3556 12.9645 28.2019C13.824 27.9703 14.7025 27.8162 15.5895 27.7416C18.4498 27.4688 21.2942 27.375 23.0014 27.375C24.6739 27.375 27.6439 27.4688 30.5089 27.7416C31.3994 27.8164 32.2814 27.9711 33.1442 28.2038C33.7142 28.35 34.2551 28.485 35.0042 28.4991C35.0042 28.8969 35.1622 29.2784 35.4436 29.5597C35.7249 29.841 36.1064 29.9991 36.5042 29.9991H41.7542C42.152 29.9991 42.5336 29.841 42.8149 29.5597C43.0962 29.2784 43.2542 28.8969 43.2542 28.4991V28.4878C43.5364 28.4531 43.8029 28.3388 44.0227 28.1584C44.2425 27.978 44.4064 27.7388 44.4955 27.4688C44.5198 27.3947 45.0983 25.6097 45.4067 22.6566C45.5539 21.2344 45.5276 19.0312 45.3383 16.8956ZM9.53233 8.74781C10.2823 7.15406 11.1401 5.35031 12.6673 4.59C14.8742 3.49125 19.4483 2.99625 23.0014 2.99625C26.5545 2.99625 31.1286 3.4875 33.3355 4.59C34.8626 5.35031 35.7167 7.155 36.4705 8.74781L36.5642 8.95125C36.619 9.06707 36.6433 9.19499 36.6346 9.32284C36.6259 9.45068 36.5847 9.57417 36.5147 9.68153C36.4448 9.78889 36.3485 9.87654 36.2351 9.93612C36.1216 9.9957 35.9948 10.0252 35.8667 10.0219C32.7514 9.9375 26.1889 9.6675 23.0014 9.6675C19.8139 9.6675 13.2514 9.94406 10.1314 10.0284C10.0033 10.0318 9.87649 10.0023 9.76305 9.94268C9.64961 9.8831 9.55333 9.79545 9.48338 9.68809C9.41344 9.58073 9.37216 9.45724 9.3635 9.3294C9.35484 9.20156 9.37907 9.07363 9.4339 8.95781C9.46671 8.88844 9.5014 8.81812 9.53233 8.74781ZM10.6508 16.2131C9.03809 16.4072 7.41509 16.503 5.79077 16.5C4.79702 16.5 3.77233 16.2188 3.58202 15.3337C3.45171 14.7384 3.46577 14.4038 3.53608 14.0672C3.59514 13.7812 3.6889 13.5731 4.15765 13.5C5.3764 13.3125 6.05796 13.5478 8.05296 14.1356C9.37577 14.5247 10.3301 15.0431 10.8739 15.4537C11.1467 15.6562 11.0014 16.185 10.6508 16.2131ZM31.4051 23.9006C30.1714 24.0413 27.7039 23.9897 23.0295 23.9897C18.3551 23.9897 15.8886 24.0413 14.6548 23.9006C13.3817 23.7591 11.7589 22.5553 12.867 21.4828C13.6048 20.7759 15.3261 20.2472 17.6183 19.95C19.9105 19.6528 20.8808 19.5 23.0201 19.5C25.1595 19.5 26.0314 19.5938 28.422 19.9509C30.8126 20.3081 32.6192 20.8434 33.1733 21.4837C34.1839 22.6313 32.6773 23.7516 31.4051 23.9062V23.9006ZM42.4208 15.3328C42.2333 16.2216 41.202 16.4991 40.212 16.4991C38.5566 16.4994 36.9026 16.4037 35.2583 16.2122C34.9714 16.185 34.8383 15.6816 35.1289 15.4528C35.6642 15.0319 36.6289 14.5238 37.9498 14.1347C39.9448 13.5469 41.0951 13.3116 42.0833 13.5075C42.3242 13.5553 42.4517 13.8141 42.4667 13.9762C42.5328 14.4278 42.5173 14.8877 42.4208 15.3337V15.3328Z"
                        fill="black" />
                </svg>
                <h1 class="text-2xl ">Rentalin</h1>
            </div>
            <span>
                &copy; {{ date('Y') }}
            </span>
        </div>

        <div class="flex flex-col">
            <a href="">Beranda</a>
            <a href="{{ url('/kendaraan') }}">Kendaraan</a>
            <a href="">Tentang Kami</a>
        </div>
    </footer>
@endsection

```
### Update file `resources\views\kendaraan.blade.php`
```blade
@extends('layouts.app')
@section('content')
    <div class="mt-4">
        <div class="flex items-center justify-between  mx-6">
            <h2 class="font-semibold text-2xl">
                Pilih mobil yang cocok untuk kamu.
            </h2>
        </div>

        <div class="grid grid-cols-3 gap-3">
            @for ($i = 0; $i < 6; $i++)
                <div class="shadow-md">
                    <img src="{{ asset('gambar/honda-brio.png') }}" class="h-52 w-2/3 object-cover mx-auto" />
                    <div class="p-4">
                        <div class="flex justify-between">
                            <h3 class="font-semibold text-xl">
                                Honda Brio
                            </h3>
                            <p>
                                Rp125.000/hari
                            </p>
                        </div>
                    </div>
                    <a class="text-center block bg-purple-800 m-2 text-white rounded-lg py-2">
                        Sewa Sekarang
                    </a>
                </div>
            @endfor
        </div>

    </div>
@endsection

```
