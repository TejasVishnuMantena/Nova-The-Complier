# 🚀 Nova Compiler

### A Custom Programming Language Compiler Built Using Java, ANTLR4, and C Code Generation

Nova Compiler is an educational compiler project developed to demonstrate the complete journey of a program from source code to executable output. The project combines fundamental Compiler Design concepts with practical implementation, providing a hands-on understanding of how modern compilers work internally.

Rather than focusing only on theory, Nova Compiler showcases each major compilation phase, including parsing, semantic analysis, intermediate code generation, and native code execution.

---

# 🎯 Project Objective

The primary goal of this project is to understand and implement the core stages of compiler construction in a simplified yet effective manner.

The compiler takes programs written in the Nova language, validates them, generates intermediate code, converts that code into C, and finally produces an executable program using GCC.

This project serves as an excellent learning resource for students studying:

* Compiler Design
* Programming Language Concepts
* System Software
* Language Processing
* Code Generation Techniques

---

# ⚙️ How Nova Compiler Works

The compiler follows a multi-stage compilation pipeline:

```text
Nova Source Program
        ↓
Lexical Analysis
        ↓
Syntax Analysis
        ↓
Parse Tree Generation
        ↓
Semantic Analysis
        ↓
Symbol Table Creation
        ↓
Three Address Code (TAC)
        ↓
C Code Generation
        ↓
GCC Compilation
        ↓
Native Executable Program
```

Each stage contributes to transforming a high-level Nova program into executable machine-level output.

---

# 📂 Project Structure

## 📌 Main.java

The entry point of the compiler.

### Responsibilities

* Reads the Nova source program.
* Initializes the lexer and parser.
* Generates and displays the parse tree.
* Starts semantic analysis.
* Displays the symbol table.
* Displays generated Three Address Code (TAC).
* Invokes the C code generator.
* Compiles generated C code using GCC.
* Executes the final binary.

This file acts as the controller that coordinates the entire compilation process.

---

## 📌 TACGeneratorVisitor.java

The core component of the compiler.

### Responsibilities

* Traverses the parse tree.
* Performs semantic validation.
* Manages variable scopes.
* Performs type checking.
* Detects semantic errors.
* Creates and updates the symbol table.
* Generates Three Address Code (TAC).
* Handles loops, conditions, arrays, and expressions.

This file can be considered the "brain" of the compiler since most compilation logic is implemented here.

---

## 📌 TACInstruction.java

Defines the structure of a Three Address Code instruction.

### Responsibilities

* Represents intermediate instructions.
* Stores operators and operands.
* Formats TAC instructions for display.
* Supports assignments, arithmetic operations, jumps, labels, and print statements.

This file serves as the foundation for the compiler's intermediate representation.

---

## 📌 CGenerator.java

The backend code generation module.

### Responsibilities

* Reads generated TAC instructions.
* Converts TAC into valid C code.
* Generates variable declarations.
* Handles arrays and expressions.
* Generates control flow statements.
* Produces the final output.c file.

This component bridges the gap between intermediate code and executable programs.

---

# 🧠 Key Concepts Implemented

### 🔹 Lexical Analysis

Breaks the source code into tokens that can be understood by the parser.

### 🔹 Syntax Analysis

Validates whether the source code follows the grammar rules of the Nova language.

### 🔹 Parse Tree Generation

Creates a structured representation of the program based on grammar rules.

### 🔹 Semantic Analysis

Ensures that the program is logically valid.

Examples include:

* Variable declaration checking
* Scope validation
* Type compatibility checking
* Array validation

### 🔹 Symbol Table Management

Maintains information such as:

* Variable Names
* Data Types
* Scope Levels

### 🔹 Three Address Code Generation

Produces an intermediate representation of the source program that is easier to optimize and translate.

### 🔹 C Code Generation

Converts TAC instructions into equivalent C code.

### 🔹 Native Program Execution

Uses GCC to compile generated C code into an executable program.

---

# 🎓 Learning Outcomes

Through this project, students can gain practical experience in:

* Compiler Construction
* Language Design
* Parse Trees and ASTs
* Semantic Analysis
* Scope Management
* Type Systems
* Intermediate Code Generation
* Backend Design
* Native Code Generation

The project provides a complete end-to-end view of how programming languages are processed and executed.

---

# 🚀 Future Enhancements

The compiler can be extended with several advanced features:

* Function Definitions and Calls
* User-Defined Classes
* String Data Type Support
* Boolean Data Types
* Compiler Optimizations
* Better Error Recovery
* Standard Library Support
* LLVM Backend Integration
* IDE Support

---

# 🏆 Conclusion

Nova Compiler is a comprehensive student-driven compiler project that demonstrates the complete compilation workflow, from parsing source code to generating executable programs.

By combining theoretical compiler concepts with practical implementation, the project serves as a strong foundation for anyone interested in understanding how programming languages are translated, analyzed, and executed behind the scenes.

---

## 👨‍💻 Author

**Developed by Tejas Vishnu Mantena**


GitHub: https://github.com/TejasVishnuMantena

