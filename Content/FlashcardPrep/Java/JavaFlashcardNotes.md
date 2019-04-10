# Java Flash Card Notes

## What is Java?

Java is a general-purpose, concurrent, object-oriented, class-based programming language that is executed using the Java Runtime Environment (JRE)

## What does JDK Stand for?

JDK stands for Java Development Kit. 

## In the case of programming languages, What is a library?

A library is a set of code that was previoulsy written, that can be called upon when building your own code.  Very usually written within the constraints of some domain.  

## What is a compiler?

A compiler is a computer program that translates human-readable code to some lower-level computer language. In the case of Java programming, Java is compiled to a low-level 'bytecode' to be executed by the Java Virtual Machine (JVM)

## What is a debugger?

a debugger is a computer program that assists in the detection and correction of errors in other computer programs.

## What tools does the Java Development Kit (JDK) contain?

 It contains the tools and libraries for development of Java programs.  It also contains compilers and debuggers needed to compile Java program.

## What is a Virtual Machine?

a Virtual Machine (VM) is a computer emulation of a computer system.  A computer whose hardware components are written entirely in software and is executed within (or above) a host  operating system.

## What does JVM stand for?

JVM stands for Java Virtual Machine.

## What is the Java Virtual Machine (JVM)?

The Java Virtual Machine (JVM) is an abstract machine that executes Java Bytecode. 

## Is  a JVM platform dependent?

Yes. Because the JVM is a virtual machine, it's interface to each host operating system must be unique.

There are different JVM for different hardware and software platforms. 

## What is the JVM responsible for?

The JVM is responsible for loading, verifying and executing the Bytecode on a platform

## What does JRE stand for?

 JRE stands for Java Runtime Environment.

## What is the Java Runtime Environment (JRE)?

The JRE provides runtime libaries and the JVM that is required to run a Java program.

## What is the shorthand 'memory' used for in programming?

'Memory' is shorthand for Random-Access Memory or RAM.  It is a form of computer data storage that stores data and machine code that is currently being used.

## What does a computer's CPU (Central Processing Unit) do?

The CPU schedules and executes instuctions; 
    - it reads and writes to memory, 
    - adds one number to another,
    - compares numbers,
    - dispatches hardware resource requests,
    - jumps to another place in the instruction set, but only if some test is true (e.g. if one number is bigger than another)

## What is a computer Thread?

A thread, or, thread of execution, is the smalles sequence of programmed instructions that can be managed independently by a scheduler

## What is an Operating System?

It is software that supports a computer's basic functions, such as scheduling tasks, executing applications, and controlling peripherals.

## What is a computer Process?

A process referes to an instance of a computer program that is being executed. Depending on the operating system (OS), a process may be made up of multiple threads of execution to be processed by multiple CPU cores concurrently.

## What does 'scheduling' mean in computing?

Scheduling is the method by which work is assigned to resources that complete the work.  The work may be virtual computation elemetns such as threads, processes, or data flows, which are in turn scheduled onto hardware resources such as processors, network links, or expansion cards.

## In Java programming, what is a method?

A method is a set of code which is referred to by name and can be called at any point in a program simply by using the method's name.

## In Java programming, what is an Object?

It is a basic conceptual real-life-inspired unit created programmatically that consists of; **state and properties** of the object, **Behaviors** (methods) and **responses** given to other objects, and an object also has a **Unique Identity**

## In Java, what is a class?

a class is a blueprint, or template for creating different types of objects in Java.

## What is the component of JVM that is used to load class files and is a memory area allocated by the JVM?

ClassLoader

## What is a Class Constant Pool?

an index of symbolic references to a Class's defined methods and properties

## What is the Runtime Constant Pool?

a JVM specific data structure, held in memory, that maps to a Class's Constant Pool

## What area of memory, allocated by the JVM,  stores per-class structures such as the runtime constant pool, field and method data, and the code for methods?

the Class (Method) Area

## What memory area is allocated by the JVM runtime and contains the runtime data area in which object instances are allocated?

the Heap

## What is a variable?

a piece of memory that can contain a data value.

## What memory area is allocated by the JVM and stores local variables and partial results at runtime?

the Stack
*It lso helps in method invocation and return value.  Each thread creates a private JVM stack at the time of thread creation*

## What memory area is allocated by the JVM that contains the address of the Java Virtual Machine instruction that is currently being executed?

the Program Counter Register

## In Java, what is a Native Method?

a native method is a method or class who's implmentation is written in another programming language such as C, C++, etc.

## What area of memory is allocated by the JVM that is reserved for all the native methods used in the application?

the Native Method Stack

## What are the different types of memory areas allocated by the JVM scheduler?

In Java, JVM allocates memory to different processes, methods and objects.  Some of the memory areas allocated by the JVM are: ClassLoader, Class (Method) Area, Heap, Stack, Program Counter Register, Native Method Stack

## What is the JIT compiler?

the Just In Time (JIT) compiler is used for performance improvements in Java.   It is enabled by default.  It is a method of compilation that occurs at execution time rather than beforehand.
