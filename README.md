# Static Site Generator

This project is a follow-through of Boot.dev's course on Static Site Generator and Functional Programming, designed to convert markdown content into HTML files, enabling easy creation of static websites. The generator incorporates Python scripts for processing markdown and managing templates, offering a modular and extendable approach.

## Features

- **Markdown Parsing**: Converts `.md` files into HTML pages.
- **Template System**: Uses a base HTML template (`template.html`) for consistent styling.
- **Static File Handling**: Copies static files like CSS and images to the output directory.
- **Automated Testing**: Includes test scripts for ensuring functionality and reliability.
- **Modular Design**: Features scripts that can be modified and extended for custom workflows.

## File Overview

### Root Files
- **main.sh**: A shell script for orchestrating the generation process.
- **template.html**: HTML template used for generating site pages.
- **test.sh**: Script for running all test cases.

### Content Files
- `content/index.md`: Main markdown file for the site's home page.
- `content/majesty/index.md`: Additional markdown file for the "Majesty" section.

### Source Files (Under `src/`)
- **copystatic.py**: Handles copying of static files (e.g., CSS, images) to the output directory.
- **gencontent.py**: Processes markdown content and generates HTML pages.
- **htmlnode.py**: Represents HTML nodes for flexible document generation.
- **inline_markdown.py**: Processes inline markdown formatting (e.g., bold, italics).
- **main.py**: The main script to coordinate the site generation process.
- **markdown_blocks.py**: Handles block-level markdown elements like headers and lists.
- **textnode.py**: Manages text nodes within the HTML structure.

### Test Files
- **test_gencontent.py**: Tests the functionality of `gencontent.py`.
- **test_htmlnode.py**: Tests HTML node creation and management.
- **test_inline_markdown.py**: Tests inline markdown parsing.
- **test_markdown_blocks.py**: Tests block-level markdown parsing.
- **test_textnode.py**: Tests text node handling.

### Static Files
- **static/index.css**: The main stylesheet for the generated site.
- **static/images/rivendell.png**: Sample image for use in the site.

## Requirements
- Python 3.x
- Markdown parser library (if not built-in)

To install required Python packages, if any:
```
pip install -r requirements.txt
```
How to Run
- Ensure all required dependencies are installed.
- Run the shell script to generate the site:
```
sh main.sh
```
The generated static site will be located in the output directory.

Purpose:

This project demonstrates the principles of modular programming and file processing in Python. It serves as a practical example of building and managing static websites programmatically.
