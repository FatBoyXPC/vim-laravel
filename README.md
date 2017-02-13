# ![Laravel.vim](https://noahfrederick.com/pi/vim-laravel-888by140-40a40a.png)

Vim support for [Laravel/Lumen 5+][laravel] projects. [![Release][release]](https://github.com/noahfrederick/vim-laravel/releases)

> :warning: This is a prerelease version, which may introduce breaking changes.

[laravel]:  https://laravel.com/
[release]:  https://img.shields.io/github/tag/noahfrederick/vim-laravel.svg?maxAge=2592000

## Features

* The `:Artisan` command wraps `!php artisan` with intelligent completion.
* Automatically edit new files generated by `:Artisan make:*` commands.
* Navigation commands (requires [projectionist.vim][projectionist]):

| Command               | Applies to...                  |
|-----------------------|--------------------------------|
| `:{E,S,V,T}asset`     | Anything under `assets/`       |
| `:Ebootstrap`         | Bootstrap files in `boostrap/` |
| `:Ecommand`           | Console commands               |
| `:Econfig`            | Configuration files            |
| `:Econtroller`        | HTTP controllers               |
| `:Edoc`               | The `README.md` file           |
| `:Eenv`               | Your `.env` and `.env.example` |
| `:Eevent`             | Events                         |
| `:Eexception`         | Exceptions                     |
| `:Efactory`           | Model factories                |
| `:Ejob`               | Jobs                           |
| `:Elanguage`          | Messages/translations          |
| `:Elib`               | All class files under `app/`   |
| `:Elistener`          | Event listeners                |
| `:Emiddleware`        | HTTP middleware                |
| `:Emigration`         | Database migrations            |
| `:Enotification`      | Notifications                  |
| `:Epolicy`            | Auth policies                  |
| `:Eprovider`          | Service providers              |
| `:Erequest`           | HTTP form requests             |
| `:Eroutes`            | HTTP routes files              |
| `:Eseeder`            | Database seeders               |
| `:Etest`              | All class files under `tests/` |
| `:Eview`              | Blade templates                |

* Enhanced `gf` command works on class names, template names, config and translation keys.
* Use `:Console` to fire up a REPL (`artisan tinker`).

## Installation

Laravel.vim has optional dependencies on [composer.vim][vim-composer],
[dispatch.vim][dispatch] (the `:Console` command), and
[projectionist.vim][projectionist] (navigation commands):

	Plug 'tpope/vim-dispatch'
	Plug 'tpope/vim-projectionist'
	Plug 'noahfrederick/vim-composer'
	Plug 'noahfrederick/vim-laravel'

## Credits and License

Thanks to Tim Pope for [rails.vim][rails] on which Laravel.vim is modeled.

Copyright © Noah Frederick. Distributed under the same terms as Vim itself.
See `:help license`.

[vim-composer]: https://github.com/noahfrederick/vim-composer
[projectionist]: https://github.com/tpope/vim-projectionist
[dispatch]: https://github.com/tpope/vim-dispatch
[rails]: https://github.com/tpope/vim-rails
