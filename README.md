📝 PicoC Interpreter: A Mini C Compiler Design Project ⚙️

The PicoC Interpreter is a mini C interpreter designed to parse, interpret, and execute C-style expressions and code snippets. It leverages fundamental compiler design principles, including lexical analysis (tokenizing), parsing, and abstract syntax tree (AST) generation, to evaluate user-provided code. The project includes a web-based front-end and a Python-based back-end, making it a full-stack application that demonstrates a comprehensive understanding of language processing and web development.

Key Features
Lexical Analysis: The interpreter performs tokenization to break down the input source code into a stream of tokens, such as identifiers, keywords (int), operators (+, -, *, /, =), and literals.

Parsing and AST Generation: It constructs an Abstract Syntax Tree (AST) from the token stream. The AST represents the hierarchical structure of the code, which is then used for evaluation.

Expression Evaluation: The interpreter can evaluate arithmetic expressions involving addition, subtraction, multiplication, and division.

Variable Assignment: It supports the declaration and assignment of integer variables. The 

main function in picoc_web.c shows a simple example where a variable a is assigned the result of 55+88.

User Interface: A web-based front-end (index.html) allows users to either upload a .txt file containing PicoC code or write code directly in an integrated editor.

Backend Services: A Flask-based back-end (backend.py) handles the compilation and execution of the C interpreter. It receives code or files, saves them, runs the picoc_web.exe executable, and returns the output to the front-end.

Technologies Used
C: The core interpreter logic, including the lexer, parser, and evaluator, is implemented in C (picoc_web.c).

Python (Flask): The back-end server is built with Flask to manage web requests, file uploads, and execute the C interpreter as a subprocess.

HTML/CSS/JavaScript: The front-end user interface is a single-page web application (index.html) using standard web technologies. It also incorporates libraries like CodeMirror for the code editor and Prism for syntax highlighting.

CORS: The Flask back-end is configured with CORS to handle cross-origin requests from the front-end.

How to Run
Clone the repository.

Ensure you have a C compiler (like GCC) and Python installed.

Install Python dependencies: pip install Flask Flask-Cors.

Start the back-end server: python backend.py.

Open index.html in your web browser to access the user interface.
