###The reasons for using Rust

Mozilla is the company known for its mission to develop tools for and drive the open standards web, most notably through its flagship browser Firefox. Every browser today, including Firefox, is written in C++, millions of lines of C++.  This provides for a fast program, with much control over memory, but it is inherently unsafe: if the code is written without the utmost programming discipline on the part of the developers, program crashes, memory leaks, segmentation faults, buffer overflows and null pointers can occur at program execution, sometimes exploitable as security breaches. 
On the other side we have Haskell, which is widely known to be a very safe and reliable language, but with very little or no control at the level of memory allocation and other hardware resources. We can plot different languages along this axis, and it seems that when a language is safer, it loses low-level control; and the inverse seems also true: a language that gives more control over resources provides much less safety.

Rust (http://www.rust-lang.org/) is made to overcome this dilemma by providing:
*	deep control over low-level resources (as much as C/C++), so it runs close to the hardware;
*	and high safety through its strong type system;


This is the unique selling point of Rust: it breaks the safety-control/speed dichotomy that, before Rust, existed among programming languages; with Rust they can be achieved together.
Rust can accomplish both these goals without a garbage collector, in contrast to most modern languages like Java, C#, Python, Ruby, Go, and the like; but optionally a garbage collector can be used. Rust is a compiled language: the strict safety rules are enforced by the compiler, so they do not cause runtime overhead. This very important part of the compiler engine is called the borrow checker, for reasons that will become clear in later chapters.
As a consequence Rust can work with a minimal runtime, or even no runtime at all, so it can be used for real-time or embedded projects, and it can easily integrate with other languages or projects.
Rust is meant for developers and projects where performance and low-level optimizations are important, but where also a safe and stable execution environment is needed. And moreover Rust adds a lot of high-level functional programming tools in the language, so that it feels at the same time as a low-level and a high-level language. 

