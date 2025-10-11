# Documentation

All documentation should be written **in English**.

Good documentation helps others understand your project - its purpose, technologies, setup, and usage. Write with the goal of enabling anyone (including new contributors) to learn what the project is about and how to use it.

## Where to Keep Documentation

Documentation can be stored in two ways:

1. **Inside the project repository** — usually in a `docs/` subfolder. This is preferred for small or medium-sized projects.
2. **In a separate repository** — if the documentation covers multiple projects or becomes large and complex (e.g., many files or diagrams). Keeping it separate can help maintain better organization and clarity.

## How to structure the documentation

For smaller projects, a single `README.md` file at the repository root is often enough.  
However, the root README should only provide a **high-level overview** — not every detail.

For larger projects, move detailed documentation into a dedicated **`docs/` folder**.  
Inside it, create a new `README.md` file as the entry point to the documentation, linking to other relevant files.

### Example

Consider such repo structure
```
README.md
docs/
	README.md
	first_time_setup.md
	usage.md
	...

...
```

- **Root `README.md`** - Explains what the project is, what it does, and links to the full documentation.
- **`docs/README.md`** - Serves as the main index or “table of contents” for all other documentation files.
- **Other files** - Contain detailed information about setup, configuration, usage, architecture, etc.
- **Subfolders** - Can be created within `docs/` for better organization when needed.

If images (or GIFs, etc) are needed as part of the documentation - they should be put inside `docs/assets/` folder, to separate them from the `.md` files.

## Markdown

All documentation should be written using **Markdown (`.md`)** files.

It's simple, easy to read even raw (not-formatted), and fully supported by GitHub. 

Read more about MD [here](https://www.markdownguide.org/).

## MD editor

To edit/read `.md` files we highly recommend Obsidian.md application (find it here: [link](https://obsidian.md/)).

It's free and fantastic application, which formats the text while you're writing it. This is especially useful for documents repositories (like this one!) - where the main purpose of the repo is to keep .md files.

Alternatively - any modern IDE supports MD syntax. Either out-of-the box, like PyCharm and VS Code, or by installing one plugin.

### PyCharm

In PyCharm - open a `.md` file and click the **Editor and Preview** button in the top-right corner, to get a split screen with editor on one side, and live preview of the formatted text on the other:
![[pycharm-md-editor.png]]

### VS Code

In Visual Studio Code - open a `.md` file and click the **Open Preview to the Side** button in the top-right corner, to get a split screen with editor on one side, and live preview of the formatted text on the other:
![[vs-code-md-editor.png]]