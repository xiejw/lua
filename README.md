copies of lua (especially old versions) for learning purpose.

```
v2.1 notes

  clients
      lua/strlib.c
        strlib_open
          lua_register all functions related to str

        str_find
          Return the position of the first caracter of a substring into a string
          LUA interface:
         			n = strfind (string, substring, init, end)

        str_len

        str_sub

          Return the substring of a string, from start to end
          LUA interface:
         			substring = strsub (string, start, end)

        str_lower
        str_upper

      lib/mathlib.c
      lib/iolib.c
        similar helper methods

      lua/lua.a
        main file
          register all methods and read input file.
```
