#Installing Rust

The Rust platform in binary (that is: executable) form can be downloaded from http://www.rust-lang.org/install.html. 

It exists for the three major platforms (Linux 2.6.18 or later, OS X 10.7 or greater, and Windows 7, 8, and 
Windows Server 2008 R2) in 32 and 64 bit format, and is delivered as an installer or as an archive format. 
You should use the current official stable release when doing serious professional work with Rust (at the time of 
writing this is version 1.0). If you would like to investigate or use the latest developments, install the Nightly 
build version.

On Windows double click the .exe installer to install the Rust binaries and dependencies. Some more details 
for Windows users can be found here: https://github.com/rust-lang/rust/wiki/Using-Rust-on-Windows.

On Linux and OS X the simplest way is to run the following command in your shell:
```python
curl -s https://static.rust-lang.org/rustup.sh | sudo sh
```

On OS X you can also use Homebrew, just execute brew install rust.
If you like to use a package manager on Ubuntu so that updating is automatic, go to: https://launchpad.net/~hansjorg/+archive/ubuntu/rust. 
* 1.	Install the package with: 
```python
	sudo add-apt-repository ppa:hansjorg/rust
```

* 2.	Then tell your system to pull down the latest list of software it knows about with:    
```python
sudo apt-get update
```

* 3.	Then install the version you want (for example the nightly version) with: 

```python
	sudo apt-get install rust-nightly 
```
	
You can find some more information about packages for other systems like FreeBSD and different Linux flavours here: 
https://github.com/rust-lang/rust/wiki/Doc-packages%2C-editors%2C-and-other-tools.
Rust has also been ported to Android OS on ARM processors, for more details see: 
https://github.com/rust-lang/rust/wiki/Doc-building-for-android.
For an iOS implementation see: https://github.com/rust-lang/rust/wiki/Doc-building-for-ios.

A ‘'bare metal’' stack called zinc for running Rust in embedded environments can be found at 
http://zinc.rs/; at this moment only the ARM architecture is supported.

The source code of resides on GitHub (see: https://github.com/rust-lang/rust/) and if you want to build Rust 
from source we refer you to: 
https://github.com/rust-lang/rust#building-from-source.
