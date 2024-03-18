
# Python Project Directory Creation Script

This repository contains a script for automatically setting up a basic directory structure for a new Python project. It's a handy tool for quickly starting new projects with a standard organization.

## Getting Started

These instructions will guide you through setting up the script to run from anywhere on your Mac, using Zsh as your shell.

### Prerequisites

Make sure you have Python installed on your system. This script is written for Python 3.

### Installation

1. **Clone the Repository**:
   - Clone this repository to your local machine or download the `create_project.py` script.

2. **Make the Script Executable**:
   - Add a shebang line to the top of the script if it's not already there:
     ```python
     #!/usr/bin/env python3
     ```
   - Make your script executable:
     ```bash
     chmod +x /path/to/create_project.py
     ```
   - Replace `/path/to/create_project.py` with the actual path to the script.

3. **Move the Script to a Bin Directory**:
   - Create a `bin` directory in your home folder and move the script there. This helps in keeping custom scripts organized:
     ```bash
     mkdir -p ~/bin
     mv /path/to/create_project.py ~/bin/create_project
     ```

4. **Update Your PATH**:
   - Add the `bin` directory to your PATH in your `.zshrc` file:
     ```bash
     echo 'export PATH="$HOME/bin:$PATH"' >> ~/.zshrc
     ```
   - Reload your `.zshrc` to apply the changes:
     ```bash
     source ~/.zshrc
     ```
   - Alternatively, you can close and reopen your terminal.

### Usage

With the setup complete, you can now create a new Python project structure from anywhere in your terminal:

```bash
create_project
```

The script will prompt you for a project name and create the following directory structure in your current directory:

```
my_project/
    /my_project
        __init__.py
    /tests
    README.md
    requirements.txt
    LICENSE
    setup.py
    .flake8
    .pylintrc
    /docs
    .gitignore
```

## Customization

Feel free to modify the `create_project.py` script to include or exclude files and directories as per your project needs.

## Contributing

Contributions, issues, and feature requests are welcome. Feel free to check [issues page](link-to-the-issues-page-of-your-repo) if you want to contribute.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
