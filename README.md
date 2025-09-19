# Geany Configuration for Markdown and LaTeX

This repository contains my personal configuration for using **Geany** as a lightweight editor for **Markdown** and **LaTeX** projects. It includes plugins, settings, and directory organization to improve productivity and workflow. This setup is visually optimized for a GTK environment, and the included color schemes are designed for the **Gruvbox Soft** theme.

-----

## Dependencies and Tools

For all features and the workflow to function correctly, some external tools are required or recommended:

  * **`geany`**: The base Integrated Development Environment (IDE) itself.
  * **`geany-plugins`**: A collection of official plugins that extend Geany's functionality. Several plugins in this setup depend on this package.
  * **`geany-themes`**: A set of additional color schemes, which serves as a base for the included theme customizations.
  * **`latexmk`**: Essential for the automated compilation of LaTeX documents. It is a Perl script that simplifies the generation of PDFs.
  * **`aspell`**: Used by the spell-checking plugin (**Spellcheck**). You also need to install the dictionaries for your desired languages (e.g., English and Portuguese).
  * **`kitty`**: A modern, fast, GPU-accelerated terminal emulator. Recommended for running compilation commands and managing the project efficiently.

-----

## Directory Structure

```
src/
├── colorschemes
├── filedefs
├── plugins
│   ├── addons
│   ├── filebrowser
│   ├── geanydoc
│   ├── geanygendoc
│   ├── Geany_Macros
│   ├── Geany_Numbered_Bookmarks
│   ├── git-changebar
│   ├── LaTeX
│   ├── lineoperations
│   ├── lsp
│   ├── markdown
│   ├── overview
│   ├── pohelper
│   ├── projectorganizer
│   ├── saveactions
│   │   └── persistent_untitled_documents
│   ├── spellcheck
│   ├── treebrowser
│   └── updatechecker
└── tags
templates/
└── files
```

-----

## Geany Setup for Markdown

1.  Enable the **Markdown** plugin:
      * Go to **Tools → Plugin Manager**.
      * Check the **Markdown** plugin.
2.  Use syntax highlighting for `.md` files.
3.  Optionally install the spell checker for English and Portuguese:
      * Enable the **Spellcheck** plugin in Plugin Manager.
      * Configure dictionaries in **Edit → Preferences → Editor → Spellcheck**.

-----

## Geany Setup for LaTeX

1.  Enable the **LaTeX** plugin:
      * Go to **Tools → Plugin Manager**.
      * Check the **LaTeX** plugin.
2.  Compile LaTeX files to PDF using external tools (e.g., `pdflatex` or the recommended `latexmk`).
3.  Configure shortcuts or macros in **Geany\_Macros** for common LaTeX commands.

-----

## Notes

  * All plugin settings are stored under `src/plugins`.
  * Templates for LaTeX and Markdown are in `templates/files`.
  * This setup is designed for productivity with **Geany** while editing documentation and scientific papers.
