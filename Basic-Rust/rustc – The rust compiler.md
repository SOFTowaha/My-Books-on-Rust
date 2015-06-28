###rustc – The rust compiler

The Rust installation directory containing rustc can be found on your machine in the following folder:
*	on Windows at 
```python
c:\Rust\bin
```
*	on Linux or OS X in 
```python
/usr/local/bin
```
It is automatically added to the search path for executables, so it can be run from any command-line window. 
The Rust libraries live in the rustlib subfolder of the bin directory on Windows, or in 
```python
/usr/local/lib/rustlib
```
on Linux.
The rustc command has the following format:  rustc [options] input
The options are one letter directives for the compiler after a dash, like –g or –W,  or words prefixed by a double dash,
like - -test or - -no-analysis. For some options both versions exist, for example showing Rust’'s version can be done 
with –V or - -version, which produces output like rustc 1.0.0-nightly.    
All options with some explanation are shown when invoking rustc -h. In the next section we verify our installation by 
compiling and running our first Rust program.
