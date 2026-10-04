Все задания выполнены в cmd

# Задание №1

```
pip --version
```
**Вывод:**

```
pip 26.0.1 from C:\Users\User\AppData\Local\Programs\Python\Python313\Lib\site-packages\pip (python 3.13)
```

Установка пакета 

```
pip install matplotlib
pip show matplotlib
```
**Вывод:**

```
Name: matplotlib
Version: 3.10.8
Summary: Python plotting package
Home-page: https://matplotlib.org
Author: John D. Hunter, Michael Droettboom
Author-email: Unknown <matplotlib-users@python.org>
License: License agreement for matplotlib versions 1.3.0 and later
Requires: contourpy, cycler, fonttools, kiwisolver, numpy, packaging, pillow, pyparsing, python-dateutil
Required-by: seaborn
```

Теперь попытаемся сделать тоже самое, но без менеджера пакетов Python pip

```
git clone https://github.com/matplotlib/matplotlib.git
cd matplotlib
python -m pip install . --no-deps
```
**Вывод:**

```
Processing .\.
  Installing build dependencies ... done
  Getting requirements to build wheel ... done
  Installing backend dependencies ... done
  Preparing metadata (pyproject.toml) ... error
  error: subprocess-exited-with-error

  × Preparing metadata (pyproject.toml) did not run successfully.
  │ exit code: 1
  ╰─> [608 lines of output]
      + meson setup C:\Users\User\matplotlib C:\Users\User\matplotlib\.mesonpy-hvhw0jv4 -Dbuildtype=release -Db_ndebug=if-release -Db_vscrt=md --native-file=C:\Users\User\matplotlib\.mesonpy-hvhw0jv4\meson-python-native-file.ini
      The Meson build system
      Version: 1.12.1
      Source dir: C:\Users\User\matplotlib
      Build dir: C:\Users\User\matplotlib\.mesonpy-hvhw0jv4
      Build type: native build
      Program python found: YES 3.13.5 3.13.5
      Project name: matplotlib
      Project version: 3.12.0.dev679+g3a143fc38
      C compiler for the host machine: gcc (gcc 11.2.0 "gcc (x86_64-posix-seh-rev3, Built by MinGW-W64 project) 11.2.0")
      C linker for the host machine: gcc ld.bfd 2.37
      C++ compiler for the host machine: c++ (gcc 11.2.0 "c++ (x86_64-posix-seh-rev3, Built by MinGW-W64 project) 11.2.0")
      C++ linker for the host machine: c++ ld.bfd 2.37
```
# Задание №2

```
docker pull node:24-slim
docker run -it --rm --entrypoint sh node:24-slim
npm -v
npm view express
 ```

 **Вывод:**

 ```
 
express@5.2.1 | MIT | deps: 28 | versions: 289
Fast, unopinionated, minimalist web framework
https://expressjs.com/

keywords: express, framework, sinatra, web, http, rest, restful, router, app, api

dist
.tarball: https://registry.npmjs.org/express/-/express-5.2.1.tgz
.shasum: 8f21d15b6d327f92b4794ecf8cb08a72f956ac04
.integrity: sha512-hIS4idWWai69NezIdRt2xFVofaF4j+6INOpJlVOLDO8zXGpUVEVzIYk12UUi2JzjEzWL3IOAxcTubgz9Po0yXw==
.unpackedSize: 75.4 kB

dependencies:
qs: ^6.14.0, depd: ^2.0.0, etag: ^1.8.1, once: ^1.4.0, send: ^1.1.0, vary: ^1.1.2, debug: ^4.4.0, fresh: ^2.0.0, cookie: ^0.7.1, router: ^2.2.0, accepts: ^2.0.0, type-is: ^2.0.1, parseurl: ^1.3.3, statuses: ^2.0.1, encodeurl: ^2.0.0, mime-types: ^3.0.0, proxy-addr: ^2.0.7, body-parser: ^2.2.1, escape-html: ^1.0.3, http-errors: ^2.0.0, on-finished: ^2.4.1, content-type: ^1.0.5, finalhandler: ^2.1.0, range-parser: ^1.2.1
(...and 4 more.)

maintainers:
- wesleytodd <wes@wesleytodd.com>
- jonchurch <npm@jonchurch.com>
- ctcpip <c@labsector.com>
- ulisesgascon <ulisesgascondev@gmail.com>
- sheplu <jean.burellier@gmail.com>

dist-tags:
latest: 5.2.1
latest-4: 4.22.3

published 10 months ago by jonchurch <npm@jonchurch.com>

 ```