<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github.com/mealet/hiw/assets/110933288/dc24f25f-707e-472d-8305-f66a6d147670">
    <source media="(prefers-color-scheme: light)" srcset="https://github.com/mealet/hiw/assets/110933288/0cf160ac-ec86-4e24-8b15-05d732c712a6">
    <img src="https://github.com/mealet/hiw/assets/110933288/0cf160ac-ec86-4e24-8b15-05d732c712a6" width="50%"/>
  </picture>

  [Release] | [Quick Start] | [Installation] | [Documentation] | [Editors Support] | [License]

  This is a simple programming language with variables, functions and manually byte-code controlling
</div>

[Release]: https://github.com/mealet/hiw/releases/latest
[Installation]: https://github.com/mealet/hiw/tree/master?tab=readme-ov-file#installation
[Quick Start]: https://github.com/mealet/hiw/tree/master?tab=readme-ov-file#quick-start
[Documentation]: https://github.com/mealet/hiw
[Editors Support]: https://github.com/mealet/hiw/tree/master?tab=readme-ov-file#editors-support
[License]: https://github.com/mealet/hiw/LICENSE

## Quick Start
Steps to start writing on hiw-lang:
1. **Install** language (see in [Installation])
2. Create file with `.hiw` extension
3. Write your first program:

```cpp
// example.hiw

// Hello World program
print("Hello World!");

// Creating variables
a = 1;
b = 2;
c = a + b;

str1 = "Hello, ";
str2 = "World!";
print(str1 + str2);

// If/Else constructions
a = 1;
if (a < 5) {
  print("less");
} else {
  print("bigger");
};

// Create functions
define foo(x) {
  print(x);
};

a = 2;

foo(1);
foo(a);

// Use functions on variables too!

a.foo();

// Use dynamic arrays
arr = [1, "string", true];

// Use cycle
a = 0;
while (a < 5) {
  print(a);
  a = a + 1;
};
```
4. Compile and run it:
```
hiw example.hiw
```
5. Compile it to binary file:
```
hiw example.hiw output
./output
```

## Installation
To correctly install **hiw language** use this instructions:
1. Install Rust from [official site](https://www.rust-lang.org/)
2. Download **hiw** from [latest release][Release]
3. Add directory where you moved binary file to PATH:
```
PATH=$PATH:/path/to/hiw/ // bash and zsh
fish_add_path "/path/to/hiw/" // fish
$env:Path += ";C:\path\to\hiw" // powershell 
```
4. Restart the terminal and type `hiw` command. You'll see instructions about using compiler.
5. Write code!

## Editors Support
Editors which supports **hiw-lang** syntax:
* [Neovim](https://github.com/mealet/hiw/blob/master/syntax-highlight/neovim/Neovim%20Syntax%20Support.md)
* [VS Code](https://marketplace.visualstudio.com/items?itemName=mealet.hiw-language)
