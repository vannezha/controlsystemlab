# How to run this project
This is a cseits website development project either control and automation laboratory or system and cybernatics laboratory. This project uses laravel as the main framework and nodejs as support for additional packages. The package we use is laravel sail to solve the problem of different dependencies using docker, laravel breeze to solve authentication problems and yarn to solve development process problems. We can run this project without any problem if we have same version package otherwise we suggest to try laravel sail to avoid any possible package conflicts. The following is the package version that we use.
- PHP:8.1.11
- Laravel:9.34.0
- Yarn:1.22.19
- Mysql:8.0.30

# Laravel Sail
See installation guide [here](https://laravel.com/docs/9.x/sail). To install laravel sail we need docker, here is a useful link if we want to install docker ([Windows](https://sh-tsang.medium.com/tutorial-docker-installation-in-wsl-2-of-windows-f4471fc3e1d4), [Linux](https://docs.docker.com/engine/install/ubuntu/), [MacOS](https://docs.docker.com/desktop/install/mac-install/)). If you use windows you need install wsl and linux distros as well. After that we need any [composer](https://getcomposer.org/) version.

# Run
* clone this project [https://github.com/vannezha/controlsystemlab.git](https://github.com/vannezha/controlsystemlab.git)
* install package using composer via terminal/powershell
  ```
  composer install --ignore-platform-req=ext-fileinfo
  ```
* make .env file and copy .env.example content to .env then save it
* (optional) if we on linux maybe we need give permission to the this whole folder
  ```
  sudo chmod 777 -R .
  ```
* open our terminal and run this command to build laravel sail, for windows just open powershell and enter bash mode and do the same thing.
  ```
  vendor/bin/sail up
  ```
  if there is problem about permission, try to give root access using sudo and wait until the process is complete
  ```
  sudo vendor/bin/sail up
  ```
* open localhost:80 as our main host, and localhost:8001 as our phpmyadmin

# more
for further sail command please read the original documentation [here](https://laravel.com/docs/9.x/sail)

<!-- <p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## About Laravel

Laravel is a web application framework with expressive, elegant syntax. We believe development must be an enjoyable and creative experience to be truly fulfilling. Laravel takes the pain out of development by easing common tasks used in many web projects, such as:

- [Simple, fast routing engine](https://laravel.com/docs/routing).
- [Powerful dependency injection container](https://laravel.com/docs/container).
- Multiple back-ends for [session](https://laravel.com/docs/session) and [cache](https://laravel.com/docs/cache) storage.
- Expressive, intuitive [database ORM](https://laravel.com/docs/eloquent).
- Database agnostic [schema migrations](https://laravel.com/docs/migrations).
- [Robust background job processing](https://laravel.com/docs/queues).
- [Real-time event broadcasting](https://laravel.com/docs/broadcasting).

Laravel is accessible, powerful, and provides tools required for large, robust applications.

## Learning Laravel

Laravel has the most extensive and thorough [documentation](https://laravel.com/docs) and video tutorial library of all modern web application frameworks, making it a breeze to get started with the framework.

You may also try the [Laravel Bootcamp](https://bootcamp.laravel.com), where you will be guided through building a modern Laravel application from scratch.

If you don't feel like reading, [Laracasts](https://laracasts.com) can help. Laracasts contains over 2000 video tutorials on a range of topics including Laravel, modern PHP, unit testing, and JavaScript. Boost your skills by digging into our comprehensive video library.

## Laravel Sponsors

We would like to extend our thanks to the following sponsors for funding Laravel development. If you are interested in becoming a sponsor, please visit the Laravel [Patreon page](https://patreon.com/taylorotwell).

### Premium Partners

- **[Vehikl](https://vehikl.com/)**
- **[Tighten Co.](https://tighten.co)**
- **[Kirschbaum Development Group](https://kirschbaumdevelopment.com)**
- **[64 Robots](https://64robots.com)**
- **[Cubet Techno Labs](https://cubettech.com)**
- **[Cyber-Duck](https://cyber-duck.co.uk)**
- **[Many](https://www.many.co.uk)**
- **[Webdock, Fast VPS Hosting](https://www.webdock.io/en)**
- **[DevSquad](https://devsquad.com)**
- **[Curotec](https://www.curotec.com/services/technologies/laravel/)**
- **[OP.GG](https://op.gg)**
- **[WebReinvent](https://webreinvent.com/?utm_source=laravel&utm_medium=github&utm_campaign=patreon-sponsors)**
- **[Lendio](https://lendio.com)**

## Contributing

Thank you for considering contributing to the Laravel framework! The contribution guide can be found in the [Laravel documentation](https://laravel.com/docs/contributions).

## Code of Conduct

In order to ensure that the Laravel community is welcoming to all, please review and abide by the [Code of Conduct](https://laravel.com/docs/contributions#code-of-conduct).

## Security Vulnerabilities

If you discover a security vulnerability within Laravel, please send an e-mail to Taylor Otwell via [taylor@laravel.com](mailto:taylor@laravel.com). All security vulnerabilities will be promptly addressed.

## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT). -->
