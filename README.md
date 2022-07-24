# Bytecode Error Handler

Handles Errors for Roblox's `Luau Compilers`, and also works for `Script into Bytecode` compilers as well.

# Instructions

Insert `Handler.cpp` into your execute code, after serializing is finished, here's an example:
```cpp
std::string Script = Luau::compile("print'Hello world!'")
/* Script now has the serialized code */
std::cout << CatchScriptError(Script) << std::endl;
```
In the debug console, the error will be displayed, and it can be modified to different text as well.

Do not change **any** of the error messages because the compiler was made to check for that error.

**Please** do credit me if you are going to public release this, or privately release this as well.

**Note: This has to be one of the ways on how to do it, you can also use `luau_load` which is better.**

**Some errors are advanced and not all errors can be accurately checked and returned.**

**Make sure your script is after serializing process! Do not input an actual script!**

I just **wanna** say this is probably the worst method ever developed, I made this for starters who are still learning or developing a compiler. You can use `luau_load` or `luaL_loadbuffer` it is **100** times better then this crap.
