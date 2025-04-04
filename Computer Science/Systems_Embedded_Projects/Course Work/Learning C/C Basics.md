###  1. Structure of a C Program

```c
#include <stdio.h>    // Preprocessor directive

int main() {          // Main function: entry point
    printf("Hello, World!\n");  // Function call
    return 0;         // Exit status
}
```

---

###  2. Data Types

| Type      | Keyword  | Example                         |
| --------- | -------- | ------------------------------- |
| Integer   | `int`    | `int x = 10;`                   |
| Character | `char`   | `char c = 'A';`                 |
| Float     | `float`  | `float f = 3.14;`               |
| Double    | `double` | `double d = 3.14159;`           |
| Void      | `void`   | For functions returning nothing |

---

###  3. Variables & Constants

```c
int age = 25;               // Variable
const float PI = 3.14f;     // Constant
```

---

###  4. Input & Output

```c
int x;
scanf("%d", &x);         // Input
printf("x = %d\n", x);   // Output
```

|Format Specifier|Type|
|---|---|
|`%d`|int|
|`%f`|float|
|`%lf`|double|
|`%c`|char|
|`%s`|string|

---

###  5. Operators

- **Arithmetic**: `+`, `-`, `*`, `/`, `%`
    
- **Relational**: `==`, `!=`, `>`, `<`, `>=`, `<=`
    
- **Logical**: `&&`, `||`, `!`
    
- **Assignment**: `=`, `+=`, `-=`, etc.
    

---

###  6. Control Structures

#### if-else

```c
if (x > 0) {
    // true block
} else {
    // false block
}
```

#### switch-case

```c
switch (value) {
    case 1: printf("One"); break;
    case 2: printf("Two"); break;
    default: printf("Other");
}
```

#### Loops

```c
for (int i = 0; i < 5; i++) { printf("%d", i); }
while (condition) { /* ... */ }
do { /* ... */ } while (condition);
```

---

###  7. Functions

```c
int add(int a, int b) {
    return a + b;
}
```

---

###  8. Arrays

```c
int arr[5] = {1, 2, 3, 4, 5};
```

---

###  9. Strings

```c
char name[] = "Alice";
```

Use `#include <string.h>` for string functions:

- `strlen()`, `strcpy()`, `strcmp()`, `strcat()`
    

---

###  10. Pointers

```c
int x = 5;
int *p = &x;      // Pointer to x
printf("%d", *p); // Dereferencing
```

---

###  11. Structs

```c
struct Person {
    char name[20];
    int age;
};
```

---

###  12. File I/O

```c
FILE *fp = fopen("file.txt", "r");
fscanf(fp, "%d", &x);
fclose(fp);
```

---
### ✅ List of C Keywords

- `auto`  
- `break`  
- `case`  
- `char`  
- `const`  
- `continue`  
- `default`  
- `do`  
- `double`  
- `else`  
- `enum`  
- `extern`  
- `float`  
- `for`  
- `goto`  
- `if`  
- `int`  
- `long`  
- `register`  
- `return`  
- `short`  
- `signed`  
- `sizeof`  
- `static`  
- `struct`  
- `switch`  
- `typedef`  
- `union`  
- `unsigned`  
- `void`  
- `volatile`  
- `while`
