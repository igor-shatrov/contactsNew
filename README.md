cd src
composer create-project laravel/laravel .
composer require laravel/ui
php artisan ui vue
npm install
npm run dev

#add in welcome.blade:
<meta name="csrf-token" content="{{ csrf_token() }}">
<script src="{{ asset('js/app.js') }}" defer></script>
#and:
<div id="app">
    <example-component></example-component>
</div>