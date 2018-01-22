Frontend(Parsers), backend(Target hardware arch),  middle(Intermediate Representation => optimzations independent)

Ahead-Of-Time (AOT) compilation is the act of compiling a programming language C intermediate representation CLI<br>
into a native machine code so that the resulting binary file can execute **natively*.<br>

Intermediate code to machine code coversion while the intermediate code is executing slows an application's performance.<br>
Ahead-of-time compiling eliminates the need for this step by occurring before execution rather than during execution.<br>
AOT produces machine optimized code, just like a standard native compiler. <br>


Interpreter => translates high level code => pre compiled code (fixed)                                  [Slow]

JIT = AOT + interpretation <br>

A common implementation of JIT compilation is to first have AOT compilation to bytecode (virtual machine code),<br>
known as bytecode compilation, and then have JIT compilation to machine code (**dynamic compilation**),<br>
**rather than **interpretation** of the bytecode.<br>
This improves the runtime performance compared to interpretation, at the cost of lag due to compilation.<br>

JIT = translates high level code => compiles small code(dynamic) and cache it(to make it fast).          [Fast]


Low level language => assembler and disassembler.


GCC, LLVM
