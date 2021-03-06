1. Firmware is software which is intended not to change once shipped. It's stored in ROM or non - volatile memory. Firmware is used in monitoring, data manupulation systems. Example - BIOS, remote control, washing machine timer etc. Firmware can be updated using complex method to refresh the memory.  

2. ROM and RAM are made up of semi-conductors (high conductivity - eases flow of current).

3. Dynamic Type language - value defines the type (PHP - $s = "abc")
4. Static Type language - datatype defines the type (Java - String s = "abc";)
5. Strongly type - Complier puts some restriction on type change (example C)
6. Weekly type - Easily variable can be changed from one type to another (JavaScript - "a" == a)

7. C is preferred over C++ for firmware development since heap cannot be used here, so many library of C++ are of no use. Also, there are are many bugs in C++ library, which are mostly fixed now.
8. Imperative language - the syntax defines the order of code execution
9. Stream is term used to define unknown bytes. Streams are unknown bytes that are sent from source to destination. Contrast to this is array of fixed size.

10. Output buffer and input buffer store the output and input stream. We need to clear output buffer using fflush otherwise once buffer is full then only it will print, which may be slow. So, if you want to write immediatly then do fflush.

11. The stdout stream is buffered, so will only display what's in the buffer after it reaches a newline (or when it's told to). You have a few options to print immediately:

Print to stderr instead using fprintf:

fprintf(stderr, "I will be printed immediately");
Flush stdout whenever you need it to using fflush:

printf("Buffered, will be flushed");
fflush(stdout); // Will now print everything in the stdout buffer

setbuf(stdout, NULL);

12. C++ has reference type but C does not have it. Reference type are immutable
13. In C, printf() returns the number of characters successfully written on the output and scanf() returns number of items successfully read.

14. Escaping:

The backslash is used as a marker character to tell the compiler/interpreter that the next character has some special meaning. What that next character means is up to the implementation. For example C-style languages use \n to mean newline and \t to mean tab.

The use of the word "escape" really means to temporarily escape out of parsing the text and into a another mode where the subsequent character is treated differently.

With respect to JavaScript:
If you want to escape single quotes in a single quote string:

var string = 'this isn\'t a double quoted string';
var string = "this isn\"t a single quoted string";
//           ^         ^ same types, hence we need to escape it with a backslash
or if you want to escape \', you can escape the bashslash to \\ and the quote to \' like so:

var string = 'this isn\\\'t a double quoted string';
//                    vvvv
//                     \ ' (the escaped characters)
However, if you contain the string with a different quote type, you don't need to escape:

var string = 'this isn"t a double quoted string';
var string = "this isn't a single quoted string";
//           ^        ^ different types, hence we don't need escaping


15. Qualifiers: static, register and extern are storage class and const, volatile and mutable are type qualifiers
