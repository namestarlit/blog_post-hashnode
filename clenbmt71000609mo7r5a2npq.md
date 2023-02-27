# How to Print "Hello, World!" in C

Hello, my name is Paul John, and this is my first technical blog.  
I've been reluctant to write my first blog and decided to write "How to Print "Hello, World!" in C, as my first blog (it doesn't demand much research and preparations anyway : D)

So, let's head straight to how to print "Hello, World!" in C, using a different approach.  
It is common to start your first program by printing some hellos to the console. I did the same thing (that's where sleepless nights begin :D ). I will complicate it a bit, using a different hacky approach for printing something to the console.  
  
Usually, to print "Hello, World!" to the console in C programming language, you'd use only a printf() function and pass in the string "Hello, World!" to it like this:

Let's call our first program, `hello.c`

```c
#include <stdio.h>

int main(void)
{
    printf("Hello, World!\n");

    return (0);
}
```

That's it. The next step is to compile and run the code to say Hello, to the world of programmers! And this is how you do it in the terminal using a GCC compiler.

```bash
$ gcc hello.c -o hello
$ ./hello
Hello, World!
```

Congratulations! You made it \\o/

In the above, the `gcc` is a command used to compile our `hello.c` program.

`gcc hello.c -o hello`, is like saying, "hey GCC, I want you to take my program hello.c and compile it for me and name the output as hello", and that's what it does exactly.

`./hello`, is how you execute your newly created program (executable) in bash :). What you have down there after that is "Hello, world!"; the output.

### The Hacky Way to Print "Hello, World!" in C

Programming is fun because there're several ways to achieve the same desired output. In our case, to print "Hello, World!" to the console. I will share a weird approach packed with concepts.

Let's call this hacky c program `hacky_hello.c` and this is what it looks like:

```c
#include <stdio.h>
#include <string.h>

int main(void)
{
    char hello[15];

    /* strcpy, copies a string to a hello array */
    strcpy(hello, "Hello, World!");
    printf("%s\n", hello);
    
    return (0);
}
```

That's it, and you get the same output : )

You already know how to compile a program. Go ahead and compile our `hacky_hello.c` program. I am not going to do that for you again.

The output should be:

```bash
Hello, World!
```

To get a clear understanding of how the `hacky_hello.c` program works; research string arrays, the strcpy() function, and arguments to the printf() function.

> Note: All codes are tested and they work. If you get any errors, fix them and make it work

This is the end of my first blog. Congratulations to me \\o/, and thank you for reading this :)

Paul John  
Software Engineering Student | Twitter: [iamstarlit](https://twitter.com/iamstarlit)