copies of lua (especially old versions) for learning purpose.

```
v2.1 notes

  include
    lua.h       all public apis, lua_type
    lublib.h    prototypes for the public methods in clients

  src
    opcode.h
        OpCode    virtual machine opcodes.
        Value     Object Value
        Object    Tag (lua_type) and Value
        Symbol    item in Symbol table; just Object

        macros
          get_word
          get_float
          get_code

    opcode.c
        TODO

  clients
      lua/strlib.c
        strlib_open
          lua_register all functions related to str

        str_find
          return the position of the first caracter of a substring

        str_len

        str_sub
          return the substring of a string, from start to end

        str_lower
        str_upper

      lib/mathlib.c
      lib/iolib.c
        similar helper methods

      lua/lua.a
        main file
          register all methods and read input file.
```
