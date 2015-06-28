###The trifecta of Rust: safe, performant and concurrent

Rust is not a revolutionary language with new cutting-edge features, but it incorporates a lot of proven techniques 
from older languages, while massively improving upon the design of C++ in matters of safe programming.
The Rust developers designed Rust to be a general purpose and multi-paradigm language: like C++ it is an imperative, 
structured and object-oriented language. But besides that it inherits a lot from functional languages on the one hand, 
and it incorporates the actor-model for concurrent programming. 

The typing of variables is static (because Rust is compiled) and strong. But, unlike in Java or C++, the developer is 
not forced to indicate types for everything: the Rust compiler is able to infer types in many cases. 

C and C++ are known to be haunted by a series of problems that often lead to program crashes or memory leaks, 
and which are notoriously difficult to debug and solve. Think about dangling pointers, buffer overflows, 
null pointers, segmentation faults, data races, and so on. The Rust compiler (called rustc) is very intelligent 
and can detect all these problems by analyzing your code, thereby guaranteeing memory safety. This is done by a 
mechanism called the borrow checker, retaining complete control over memory layout, but without needing the runtime 
burden of garbage collection. And of course safety also implies much less possibility for security breaches.

rustc is completely self-hosted, which means it is written in Rust and can compile itself by using a previous version. 
It uses the LLVM compiler framework as its back-end (for more info see http://en.wikipedia.org/wiki/LLVM), and produces 
natively executable code that runs blazingly fast, because it compiles to the same low-level code as C++ 
(see for example http://benchmarksgame.alioth.debian.org/u64q/rust.php). 

Because Rust compiles to native code like Go and Julia, no heavy-weight virtual machine with garbage collection is needed. 
In this respect it differs from Java and the JVM, and thus also languages that run on the JVM like Scala and Clojure, 
.NET and its CLR with C# and F#, JavaScript, Python, Ruby, Dart and so on.

For concurrency Rust adopts the well-known actor-model from Erlang. Lightweight processes called tasks perform work 
in parallel. They do not share heap memory, but communicate data through channels. These primitives make it easy for 
programmers to leverage the power of the many CPU cores available on current and future computing platforms.
Rust is designed to be as portable as C++ and to run on widely-used hardware and software platforms: at present it 
runs on Linux, Mac OS X, Windows, FreeBSD, Android and iOS. It can call C code as simple and efficient as calling 
C code from C, and conversely C code can also call Rust code.


Other Rust characteristics that will be discussed in more detail in later chapters are:
*	variables are immutable by default 
*	enums 
*	pattern matching 
*	generics 
*	higher-order functions and closures 
*	an interface system called traits 
*	a hygienic macro system 
*	zero-cost abstractions, which means: Rust has higher-language constructs, but these do not have an impact on performance.

Rust gives you ultimate power over memory allocation as well as removing many security and stability problems commonly associated with native languages.

