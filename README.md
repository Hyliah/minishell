<!-- README.md -->
<h1 align="center">
  🐚 minishell
</h1>

<p align="center">
  <code>$ ./minishell</code><br>
  <i>A bash lookalike program built from scratch as part of the 42 School curriculum. </i><br>
  <strong>Built with C — by  <a href="https://github.com/Melodycherry">@Melodycherry</a> & <a href="https://github.com/Hyliah">@Hyliah</a></strong><br>
  aka <i> Les codeuses du dimanche </i>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Language-C-pink.svg" />
  <img src="https://img.shields.io/badge/Status-Completed-violet" />
  <img src="https://img.shields.io/badge/School-42%20Lausanne-blueviolet" />
</p>

<h2>♦ Key Features ♦</h2>
<p> 

➛ Prompt display and user input handline

➛ Lexical analysis and command parsing

➛ Environment variable expansion

➛ Input/output redirections (>, >>, <, <<)

➛ Heredocs

➛ Piping (|)

➛ Builtin command handling (cd, echo, export, unset, env, exit, pwd)

➛ Signal handling (Ctrl+d, Ctrl+c, Ctrl+\)

➛ Exit status and process management
</p>

<h2>♦ Project Structure ♦</h2>

```bash
minishell/
├── main/             # Program entry and loop
├── utils/            # Utility functions
├── signals/          # Signal handling (SIGINT, SIGQUIT, etc.)
├── parsing/
│   ├── lexer/        # Tokenization of user input
│   ├── parser/       # Syntax parsing
│   └── expander/     # Variable and wildcard expansion
├── heredoc/          # Heredoc implementation (<<)
├── execution/
│   ├── redirection/  # Input/output redirections
│   ├── pipe/         # Pipe management
│   └── builtins/     # Builtin command implementations
```


<h2>♦ Team Collaboration ♦</h2>

<p>
This project was developed in close collaboration between:

<strong>Together</strong>: We co-designed the parser, lexer, and overall structure, ensuring consistent integration across all modules.

<strong>Hyliah</strong>: Focused on execution, especially pipes, heredocs, and redirection.

<strong>Melodycherry</strong>: Concentrated on builtins and signal handling.

Together from start to finish (minish)
</p>

<h2>♦ How to run ♦</h2>

```bash
git clone https://github.com/YourUsername/minishell.git
cd minishell
make
./minishell
```

<h2>♦ Exemple of commands ♦</h2>

```bash
Les codeuses du dimanche :  echo Hello World | cat -e > output.txt
Les codeuses du dimanche :  cat output.txt
Hello World$
```



