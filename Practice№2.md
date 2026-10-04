Все задания выполнены в cmd

# Задание №1

```
pip --version
```
**Вывод:**

```
pip 26.0.1 from C:\Users\User\AppData\Local\Programs\Python\Python313\Lib\site-packages\pip (python 3.13)
```

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