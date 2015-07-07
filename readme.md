# Laravel Web Installer

## Installation

First, pull in the package through Composer.

```
"require": {
    "rachidlaasri/laravelinstaller": "1.0"
}
```

And then, include the service provider within `app/config/app.php`.

```
'providers' => [
    'RachidLaasri\LaravelInstaller\Providers\LaravelInstallerServiceProvider::class,
];
```

Then, register the middleware within `app/Http/Kernel.php`.
```
    'isInstalled' => \RachidLaasri\LaravelInstaller\Middleware\IsInstalled::class,
```
## Usage

To use this package run :
```bash
php artisan vendor:publish
```

After that, you can edit :
 
 `app/config/installer.php`
 
 And the language file.