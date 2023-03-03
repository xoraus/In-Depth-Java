# Java: A High-level Overview

## What is Java & Who is Using It?

- What is Java?
  - General-purpose
  - Object-oriented
  - Platform independent
  - Concurrent
  - Very fast
  - Familiar syntax
  - Simple & Safe
  - Java: Automatic memory management.
    - C & C++: Manipulate memory to free up space
- Java is a general-purpose, object-oriented, platform-independent, concurrent programming language that runs fast
- Java's key attributes are: general-purpose, object-oriented, platform-independent, concurrent programming language, and fast
- Java is designed to be easy to use, safe, and secure
- Java provides automatic memory management through garbage collection
- Java has a rich library, the Java API, which includes pre-defined functionality for developers to use
- Java is widely adopted by large companies like Google, Netflix, and Amazon
- Java is popular in domains like search, data mining, and machine learning, which deal with large amounts of data
- Java was initially developed for embedded systems and later evolved into a popular language for developing large-scale web applications, standalone desktop applications, and mobile applications.

## Story behind Java's Creation ~ A Brief History

- Machine Language
  - Computers understand instructions
  - Program ~ set of instructions
  - Instructions ~ 0s & 1s
  - Machine language (machine code or native code)
  - e.g., 000000 00001 00010 00110 00000 100000
- Assembly Language
  - add $s0, $s1, $2
  - assembly language → assembler → machine language
- Low-level Languages
  - Machine language & assembly language
  - Use low-level details, e.g., memory location
- High-level Languages
  - FORTRAN, C, C++, Java, C#
  - Use english-like words, math notations, punctuations.
  - Hide low-level details public class.
- Goals
  - Consume less memory
  - Delivery of software components
  - Platform Independence
  - Security
  - Multi-threaded
- Compilation
  - source code → compiler → target language
  - target language
    - machine code
    - bytecode
    - programming language
  - ClojureScript into JavaScript → source-to-source compilers or transcompilers
- Core Compilation Operations
  - Verifying syntax & semantics of source code
  - Verifying syntax & semantics of source code
    - `System out.printIn("hello!");`
  - Code optimizations
  - Generate machine code
- `*7` & Initial Failure → Cable TV
- World Wide Web
- Java meets WWW
- Pre-Java ~ Static HTML
- HotJava browser at Sun SunWorld conference
  - HTML + programs (applets) = dynamic
  - Java installed in browser
  - Applets are platform independent
- Netscape Navigator ships with Java
- First version released in 1996.

- Sun Microsystems, a Silicon Valley-based company that sold Unix-based computers, created a small team called the Green team to brainstorm on the next wave in computing.
- The team concluded that a network of heterogeneous consumer devices that communicate with each other could be one significant trend, leading them to build a prototype as part of a new project called The Green Project.
- The vision for the project was to build an interactive wireless handheld device that would communicate with home entertainment devices like TV and VCR.
- The software developed by the green team would be installed on all of these devices, and it would help with activities like playing a certain TV channel or recording a particular favorite program.
- The software developed by the green team should have some unique goals, including consuming less memory, allowing devices to communicate with each other and pass around any software programs, platform independence, security, and Multithreading.
- Initially, C++ was considered for this project, but it was rejected because it did not meet some of the project goals, such as platform independence.
- James Gosling, one of the team members, created an entirely new language called Oak, which was later renamed to Java due to trademark issues.
- The Green team came up with a working demo on the interactive handheld device, which was called Star seven.
- The newly popular World Wide Web was exactly identical to the Green Project, which is a network of heterogeneous systems communicating with each other.
- Sun developed a browser called Hot Java and showcased it at the Sun World Conference in 1995, which allowed Java programs called applets to be embedded in HTML pages and made web applications interactive.
- The applet could run on heterogeneous client platforms, which is platform independence.
- Netscape also announced that their popular Netscape Navigator browser would include Java support, and soon the first version of Java was released in January of 1996.

## Platform Dependency

- Platform dependency refers to the inability to run a program on a different platform without recompiling it.
- Executable files generated on different operating systems have different formats, such as PEXE for Windows and ELF for Linux.
- Machine code generated for a program on different processors, like x86 or ARM, is different.
- Interpreters can help resolve platform dependency by translating the code into a form that can run on the target platform without recompilation.
- A demonstration is given by compiling and running a C program on both Windows and Linux, showing that the executable generated on one platform cannot be executed on the other platform.

## Interpreter

- Interpreter
  - Virtual machine
  - fetch-and-execute cycle
- Interpreter's fetch-and-execute

  - fetch next program statement
    - understand the statement
  - execute precompiled machine code in its library.

- Compiler languages like C are not platform independent.
- Interpreters address the platform dependency issue but have some limitations.
- In an interpreted language, an interpreter directly executes the source code.
- Interpreter is a program that simulates a CPU and executes the source code.
- Fetch and execute cycle is the most fundamental operation of a computer and every programmer must know it.
- Interpreter maintains a library of compile machine code, and it just executes the appropriate compile machine code that corresponds to the program statement.
- One main advantage of an interpreter is platform independence.
- Pros of an interpreter include no compensation step, enabling easier updates, and platform independence.
- Cons of an interpreter include being slower than compiled code due to costly memory access operations and having to be reinterpreted every single time it is run.

## Platform Independence in Java + Demo

- Java uses compilation and interpretation to achieve both platform independence and fast execution speed
- Java source code is compiled into Java bytecode, which is an intermediate format that is platform independent
- The compiled Java bytecode can be interpreted on any platform that has a Java interpreter installed
- The Java interpreter is the JVM, which is a virtual machine that can execute Java programs
- Java bytecode is compact and optimized to be interpreted by the JVM, which makes executing Java programs much faster than interpreting source code directly
- Just-in-time compilation is a process performed by the JVM at execution time to further optimize Java programs
- Java bytecode's compact form enables quick transfer of bytecodes across networks
- Java can be compiled and executed using the Java compiler and Java interpreter, respectively, with the same commands across different platforms

## Java Virtual Machine

- JVM is the Cornerstone of Java platform
- Core Responsibilities:
  - Loading & interpreting Java bytecode
  - Security
  - Automatic memory management
- Performance - Bytecode interpretation is much faster - Java bytecode is compact, compiled and optimized. - Just-in-tim (JIT) comilation - Identify frequently executed bytecode ~ **hotspots** - JIT comiler converts **hotspots** to machine code - Cache machine code - Cached machine code → faster execution - Also called dynamic compilation.
  ![[Java - A High-level Overview-20230304045211.png]]

- Java has unique selling point of platform independence and fast execution speed due to JVM
- JVM can interpret Java bytecode for platform independence and fast execution
- JVM can perform GI compensation for even faster execution speed
- Other languages like Scala and Groovy can be compiled to Java bytecode for platform independence and fast execution
- JVM is the cornerstone of Java and has core responsibilities of loading and interpreting Java bytecode, providing security, and automatic memory management
- Each Java application runs inside a JVM instance
- Typical JVM architecture involves loading JVM into memory, allocating Java memory, loading class with class loader, verifying bytecode with bytecode verifier, and executing bytecode with execution engine
- JVM is an abstract computing machine with Java bytecode as instruction set and manipulates memory at runtime
- JVM components include class loader, bytecode verifier, and execution engine
- Understanding JVM is important for understanding why Java programs run fast and for effective Java programming.

## An Overview of Java SE

**Java Software Family**

- Java Standard Edition (Java SE)
  - Standalone applications for desktops & servers
  - Hospital management system
- Java Enterprise Edition (Java EE)
  - Large-scale applications for servers
  - e-commerce Website
- Java Micro Edition (Java ME)
  - Applications for resource-constrained devices
  - Uses subset of Java SE

**Java SE**

- Java Language Specification (JLS)
- Java Virtual Machine Specification (JVMS)
- Java API Specification
  - Oracle JDK
  - Oracle OpenJDK
- JDK ~ Java Development Kit
  - JRE
    - JVM
    - Java API
  - Dev. Tools
- OpenJDK (API + HotSpot JVM)
- AdoptOpenJDK (OpenJ9)
- Java Language and Virtual Machine Specifications
  - Umbrella JSR
  - Java Community Process (JCP)

## Java SE Release Cycles:

- Java SE has a planned release cycle of every six months, with regular updates and security patches in between.
- Major releases happen every three years, with the first release in a new feature release line designated as a long-term support (LTS) release.

## Hello, World in Java

```java
public class HelloWorld {
   public static void main(String[] args) {
      System.out.println("Hello, World!");
   }
}
```

` javac HelloWorld.java` & `java HelloWorld`

- **main() method**
  - Program starts with main()
  - java HelloWorld
    - JVM loads bytecodes of HelloWorld.class into memory
    - Invokes main()
  - Must be declared as public, static, and void
