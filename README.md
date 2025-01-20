## CarbonBR T.I. Dev configuration

<sup>Please follow the instructions below.</sup>

## apt:

00 - Updates a list of packages: 
```
sudo apt update
```

01 - Updates all installed packages to their latest versions:
```
sudo apt full-upgrade
```

02 - Install Dependencies:
* git
* curl
* tk-dev
* xz-utils
* libffi-dev
* libssl-dev
* libbz2-dev
* zlib1g-dev
* libxml2-dev
* liblzma-dev
* libsqlite3-dev
* libxmlsec1-dev
* libreadline-dev
* build-essential
* libncursesw5-dev

```
sudo apt install git;
sudo apt install curl;
sudo apt install tk-dev;
sudo apt install xz-utils;
sudo apt install libffi-dev;
sudo apt install libssl-dev;
sudo apt install libbz2-dev;
sudo apt install zlib1g-dev;
sudo apt install libxml2-dev;
sudo apt install liblzma-dev;
sudo apt install libsqlite3-dev;
sudo apt install libxmlsec1-dev;
sudo apt install libreadline-dev;
sudo apt install build-essential;
sudo apt install libncursesw5-dev
```

## curl:

03 - Install pyenv for environment variables:
```
curl -fsSL https://pyenv.run | bash
```
04 - Config pyenv:
```
echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.bashrc
```
```
echo '[[ -d $PYENV_ROOT/bin ]] && export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.bashrc
```
```
echo 'eval "$(pyenv init - bash)"' >> ~/.bashrc
```
```
echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.profile
```
```
echo '[[ -d $PYENV_ROOT/bin ]] && export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.profile
```
```
echo 'eval "$(pyenv init - bash)"' >> ~/.profile
```
05 - Restart the Linux terminal.

```
pyenv install 3.12.6
```
## postgresql
06 - Install postgresql

```
sudo apt install -y postgresql-common;
sudo /usr/share/postgresql-common/pgdg/apt.postgresql.org.sh;
sudo apt install postgresql-16-postgis-3 postgresql-16
```
07 - Config Postgresql:
```
sudo su postgres;
psql;
```
> [!IMPORTANT]
> Don't copy and paste, read the doc ``postgresql.org sql-alteruser``
> ```
> ALTER USER postgres WITH PASSWORD 'postgres';
> ```

## npm

08 - Install npm:
```
sudo apt install npm
```
## Project commands

```
proetry install
```

```
npm install
```

```
poetry run python manage.py migrate
```

```
poetry run python manage.py runserver
```

```
npm run dev
```



