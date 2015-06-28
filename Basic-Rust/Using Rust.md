#Using Rust

It is clear from the previous sections that Rust can be used in projects that normally would use C or C++. 
Indeed many regard Rust as a successor to, or a replacement for C/C++. Although Rust is designed to be a systems 
language, due to its richness of constructs it has a broad range of possible applications, making it an ideal 
candidate for applications that fall into one or all of the following categories:

*	resource intensive systems
*	client applications, like browsers
*	low-latency high-performance systems, like device drivers, games and signal processing
*	highly distributed and concurrent systems, like server applications
*	real-time and critical systems, like operating systems or kernels
*	embedded systems (requiring a very minimal runtime foot print) or resource-constrained environments, like Raspberry Pi, Arduino or robotics
*	tools or services that can''t support the long warmup delays common in JIT (Just In Time) compiler systems and need instantaneous startup 
*	large-scale, high-performance complex software systems

Rust is especially suited when code quality is important, that is for:

*	modestly-sized or larger developer teams
*	code for long-running production use
*	code with a longer lifetime that requires regular maintenance and refactoring
*	code for which you would write more unit tests to safeguard

Dynamic languages like Ruby or Python give you the initial coding speed, but the price is paid later: in writing 
more tests, runtime crashes, or even production outages. 

The Rust compiler forces you to get a lot of things right at compile-time, which is the least expensive place to 
identify and fix bugs.
Rust’'s object orientation is not that explicit or evolved as common object-oriented languages like Java, 
C# or Python. Compared with Go, Rust gives you more control over memory and resources and so let’'s you 
code on a lower level. Go also works with a garbage collector, has no generics, and no mechanism to prevent
data-races between its goroutines used in concurrency. Julia is focused on numerical computing performance, 
works with a JIT compiler and also doesn’'t give you that low level control as Rust does.

Even at this stage two companies already use Rust in production:
*	OpenDNS (http://labs.opendns.com/2013/10/04/zeromq-helping-us-block-malicious-domains/): 
    which is a middleware tool for blocking malware and malicious domains.
*	Skylight  (https://www.skylight.io/) from the company Tilde (http://www.tilde.io/): 
    which is a tool for monitoring the execution of Rails apps.
