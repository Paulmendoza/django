# Usage

## Hatch (v1.13)
### Install
https://hatch.pypa.io/latest/install/
### Setup
```console
$ hatch python install 3.13
$ hatch env create
$ hatch run python -m pip iunstall --upgrade pip
$ hatch run python -m pip install Django==5.1.3
```

## Django
```console
$ hatch shell # enters into default shell
$ django-admin startproject --extension=ini,py,toml,yaml,yml --template=https://github.com/Paulmendoza/django-hatch-template/archive/main.zip <projectname>
$ exit # exits default venv shell
$ cd <projectname>
```

> Note: Uncomment 'static' in .gitignore file

### Scripts
```console
// while in project directory
$ hatch run dev:migrate
$ hatch run dev:runserver # Tailwind might be installed on first run
```