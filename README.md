# String Processing and Manipulation in C

String Processing and Manipulation in C is a collection of five independent console exercises focused on the fundamental techniques used to read, inspect, transform, and combine text in the C programming language. The project develops these skills through concise programs that progress from reversing a word and measuring its length to rearranging characters, joining text, and counting specific occurrences. Each exercise can be compiled and run separately, making the collection suitable for focused practice and for reviewing the essential principles of string handling.

## Exercises

| File | Objective |
| --- | --- |
| `exercise_01.c` | Read a word and print its characters in reverse order. |
| `exercise_02.c` | Determine the length of a word by examining its characters directly. |
| `exercise_03.c` | Measure a word and exchange its first and last characters. |
| `exercise_04.c` | Read two words, report their lengths, and concatenate them. |
| `exercise_05.c` | Count the lowercase `a` characters contained in a word. |

## Key Concepts

The exercises provide practical experience with:

- character arrays and null-terminated strings;
- indexed traversal and loop-based text processing;
- console input and formatted output;
- dynamic array sizes supported by C99;
- common operations from the C standard string library;
- independent compilation of programs that define separate entry points.

## Requirements

To build and run the complete collection, the system must provide:

- a terminal or command-line environment;
- GCC or Clang with support for the C99 standard.

No third-party libraries are required. The examples below use GCC. If Clang is installed instead, replace `gcc` with `clang` in each compilation command.

Confirm that the compiler is available before building the exercises:

```text
gcc --version
```

## Build Instructions

Open a terminal in the repository root, then follow the instructions for the current operating system. Each source file must be compiled separately because every exercise is an independent program.

### Windows

Use PowerShell with a GCC distribution that supports C99, such as MinGW-w64. Create the output directory:

```powershell
New-Item -ItemType Directory -Force -Path build | Out-Null
```

Compile all exercises:

```powershell
gcc -std=c99 -Wall -Wextra -pedantic exercise_01.c -o build\exercise_01.exe
gcc -std=c99 -Wall -Wextra -pedantic exercise_02.c -o build\exercise_02.exe
gcc -std=c99 -Wall -Wextra -pedantic exercise_03.c -o build\exercise_03.exe
gcc -std=c99 -Wall -Wextra -pedantic exercise_04.c -o build\exercise_04.exe
gcc -std=c99 -Wall -Wextra -pedantic exercise_05.c -o build\exercise_05.exe
```

### macOS and Linux

Create the output directory:

```bash
mkdir -p build
```

Compile all exercises:

```bash
gcc -std=c99 -Wall -Wextra -pedantic exercise_01.c -o build/exercise_01
gcc -std=c99 -Wall -Wextra -pedantic exercise_02.c -o build/exercise_02
gcc -std=c99 -Wall -Wextra -pedantic exercise_03.c -o build/exercise_03
gcc -std=c99 -Wall -Wextra -pedantic exercise_04.c -o build/exercise_04
gcc -std=c99 -Wall -Wextra -pedantic exercise_05.c -o build/exercise_05
```

## Run Instructions

Run one exercise at a time and follow the prompts displayed in the terminal.

### Windows

```powershell
.\build\exercise_01.exe
.\build\exercise_02.exe
.\build\exercise_03.exe
.\build\exercise_04.exe
.\build\exercise_05.exe
```

### macOS and Linux

```bash
./build/exercise_01
./build/exercise_02
./build/exercise_03
./build/exercise_04
./build/exercise_05
```

The commands are listed together for completeness, but each program finishes before the next one is started. They may also be invoked individually in any order.

## Input and Output

All exercises are interactive and display their prompts in Italian. When requested, enter a positive maximum length and then provide the text to process. Text input is read as a single word, so it must not contain spaces or other whitespace characters. Keep every word within the maximum length requested by the corresponding program.

Each exercise prints the entered data and the result of its operation directly to the terminal. The generated executables are stored in the `build` directory and can be removed and recreated at any time.
