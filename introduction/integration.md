# Integration

## Laravel 4

The Sentry package has optional support for Laravel 4 and it comes bundled with a Service Provider and a Facade for easy integration.

After installing the package, open your Laravel config file located at `app/config/app.php` and add the following lines.

In the `$providers` array add the following service provider for this package.

	'Cartalyst\Sentry\Laravel\SentryServiceProvider',

In the `$aliases` array add the following facade for this package.

	'Sentry' => 'Cartalyst\Sentry\Laravel\Facades\Sentry',

### Configuration

After installing, you can publish the package configuration file into your application by running the following command on your terminal:

	php artisan config:publish cartalyst/sentry

This will publish the config file to `app/config/packages/cartalyst/sentry/config.php` where you can modify the package configuration.
