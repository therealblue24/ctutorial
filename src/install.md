# Install a C compiler
To program in it, of course.

## Linux
The simplest of all. For debian-based distros:
```sh
$ sudo apt update
$ sudo apt-get install build-essential
```
If you don't use a debian-based distro, just search up how to install GCC or clang for your system's distro.

## MacOS
2nd simplest of all. First you want to install brew:
```sh
$ /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
# In the next steps of the output section, run both commands.
```
(Run the above command if you dont have brew)

Then install clang (with llvm, ofc)
```sh
$ brew update
$ brew install llvm
```
This will take a long time, but then you will have a working C compiler. Use `clang --version` to see if the compiler is working.

## Windows
Oh god uh
Installing on windows is hard, quite hard so for know you can use `https://www.onlinegdb.com/online_c_compiler`
