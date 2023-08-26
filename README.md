# Cli-sh

```
            /$$ /$$                   /$$
           | $$|__/                  | $$
   /$$$$$$$| $$ /$$          /$$$$$$$| $$$$$$$
  /$$_____/| $$| $$ /$$$$$$ /$$_____/| $$__  $$
 | $$      | $$| $$|______/|  $$$$$$ | $$  \ $$
 | $$      | $$| $$         \____  $$| $$  | $$
 |  $$$$$$$| $$| $$         /$$$$$$$/| $$  | $$
  \_______/|__/|__/        |_______/ |__/  |__/

  A minimal, customizable CLI written in shell
              cli-sh.dev | v0.3.2
```

## Installation

1. Copy the `cli` script to your project root and make it executable.

    ```sh
    chmod +x ./cli
    ```

## Usage

1. Create a `run` directory in your project.

    ```sh
    mkdir run
    ```

2. Create a script for your command in the `run` directory.

    ```sh
    echo '#!/bin/sh' >> run/hello
    echo 'echo hello world!' >> run/hello
    chmod +x run/hello
    ```
3. Run your command.

    ```sh
    ./cli run/hello
    ```

## Convention over Configuration

This minimal cli uses a convention over configuration approach. This means that
you can use it without any configuration, but you can also customize it to your
needs.

## Features

### Filesystem routing

Use transparent filesystem routing for cli command structures.

[Example](examples/filesystem-routing/README.md)

### Directory commands

Use commands with the same name as the directory to implement directory commands.

[Example](examples/directory-commands/README.md)

### Flexible commands

Use any executable or script as building blocks for your cli commands.

[Example](examples/basic/README.md)

### Shell autocompletion

Use out-of-the-box autocompletion in all shell environments.

[Example](examples/shell-autocompletion/README.md)

### Display command tree

Use the default command to display all available commands as tree.

[Example](examples/display-command-tree/README.md)

### Hooks

Use hooks to intercept, extend and alter command execution.

[Example](examples/hooks/README.md)
