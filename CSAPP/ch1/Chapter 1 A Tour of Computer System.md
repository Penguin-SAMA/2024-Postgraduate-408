# Chapter 1 A Tour of Computer System

## 1.1 Information Is Bits + Context

etc.

## 1.2 Programs Are Translated by Other Programs into Different Forms

-   The individual C statements must be translated by other programs into a sequence of low-lecel *machine-language* instructions.

-   On a Unix system, the translation from source file to object file is performed by a compiler driver:

    ![image-20230408222826953](./assets/image-20230408222826953.png)

```shell
linux> gcc -o hello hello.c
```

***preprocessor, compiler, assembler, and linker*** are known collectively as the compilation system.

-   **Preprocessing phase.** The preprocessor modifies the original C program according to directives that begin with the `#` character. The result is another C program, typically with the `.i` suffix.
-   **Compilation phase.** The compiler translates the text file `hello.i` into the text file `hello.s`, which contains an *assmbly-language program*.
-   **Assembly phase. **The assembler translates `hello.s` into machine-language instructions, packages them in a form known as a *relocatable object program*, and stores the result in the object file `hello.o`. 
-   **Linking phase.** Lingking is the process of combining object files and libraries into a single executable file or library in C programming. In `hello` program, Lingker links `printf.o` and `hello.o`. 

## 1.3 It Pays to Understand How Compilation Systems Work

