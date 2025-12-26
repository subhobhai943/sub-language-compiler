# SUB Language Compiler

<div align="center">

![SUB Language](https://img.shields.io/badge/SUB-Language-blue?style=for-the-badge)
![Version](https://img.shields.io/badge/version-1.0-green?style=for-the-badge)
![License](https://img.shields.io/badge/license-MIT-orange?style=for-the-badge)

**A modern, cross-platform programming language with blockchain-style syntax**

</div>

## 🚀 Overview

SUB Language is an innovative programming language designed for cross-platform development with embedded multi-language support. This repository contains the **pre-compiled compiler binaries** ready for distribution and use.

## 📦 What's Included

This repository contains the complete SUB Language compiler toolchain:

### Compiler Components
- **`lexer.o`** (6.7 KB) - Lexical analyzer for tokenizing SUB source code
- **`parser.o`** (4.2 KB) - Syntax parser for building abstract syntax trees
- **`semantic.o`** (3.2 KB) - Semantic analyzer for type checking and validation
- **`codegen.o`** (7.6 KB) - Code generator for producing executable output
- **`utils.o`** (6.8 KB) - Utility functions for compiler operations
- **`sub.o`** (6.0 KB) - Main compiler driver object file

### Executable
- **`sub`** (25 KB) - Complete linked compiler executable

### Examples
- **`example.sb`** - Comprehensive example demonstrating SUB Language features

## 🎯 Key Features

- **Blockchain-Style Syntax** - All statements begin with `#` for unique code structure
- **Cross-Platform UI** - Built-in UI components that work across platforms
- **Multi-Language Embedding** - Seamlessly embed Python and JavaScript code
- **Modern Language Features** - Functions, conditionals, loops, and more
- **Easy Integration** - Simple syntax for rapid application development

## 🔧 Installation

### Prerequisites
- GCC or compatible C compiler
- Linux/Unix environment (or WSL on Windows)
- Basic command-line knowledge

### Quick Start

1. **Clone the repository:**
```bash
git clone https://github.com/subhobhai943/sub-language-compiler.git
cd sub-language-compiler
```

2. **Make the compiler executable:**
```bash
chmod +x sub
```

3. **Compile your first SUB program:**
```bash
./sub example.sb
```

## 📝 SUB Language Syntax

### Variable Declaration
```sub
#var appName = "Hello SUB"
#var version = 1.0
#var userCount = 0
```

### Functions
```sub
#function calculateSum(a, b)
    #var result = a + b
    #return result
#end
```

### Conditionals
```sub
#if age >= 18
    #return "Adult"
#elif age >= 13
    #return "Teenager"
#else
    #return "Child"
#end
```

### Loops
```sub
#for i in range(1, 11)
    #print(i)
#end
```

### Cross-Platform UI
```sub
#ui.window(title="SUB Demo App", width=800, height=600)
    #ui.label(text="Welcome to SUB Language!", size=24)
    #ui.button(text="Click Me", onclick=handleClick)
    #ui.input(placeholder="Enter your name", id="nameInput")
#end
```

### Embedded Languages
```sub
# Embed Python
#embed python
    import json
    data = {"users": 100, "active": 75}
    result = json.dumps(data)
#endembed

# Embed JavaScript
#embed javascript
    const config = {
        theme: "dark",
        language: "en"
    };
    console.log(config);
#endembed
```

## 🏗️ Building from Source

If you need to rebuild the compiler:

```bash
# Link all object files
gcc -o sub sub.o lexer.o parser.o semantic.o codegen.o utils.o
```

## 📖 Usage Examples

### Basic Program
```sub
#function main()
    #print("Hello, SUB Language!")
#end

main()
```

### Run the program:
```bash
./sub myprogram.sb
```

## 🤝 Contributing

While this repository contains pre-compiled binaries, contributions to documentation and examples are welcome! For source code contributions, please visit the main SUB Language development repository.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Subho Bhai**
- GitHub: [@subhobhai943](https://github.com/subhobhai943)

## 🌟 Acknowledgments

- Built with modern compiler design principles
- Inspired by Python, JavaScript, and blockchain technology
- Designed for ease of use and cross-platform compatibility

## 📮 Support

If you encounter any issues or have questions:
- Open an issue in this repository
- Check the example.sb file for syntax reference
- Review the documentation for detailed usage

---

<div align="center">

**Made with ❤️ for developers who want simplicity with power**

</div>