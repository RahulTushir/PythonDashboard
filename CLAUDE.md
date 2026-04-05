# CLAUDE.md

This file provides guidance for AI assistants (like Claude) working on this repository.

## Repository Overview

**PythonDashboard** is a minimal learning/experimentation repository created by Rahul Tushir (2019). Despite its name, it currently contains no Python code. The repository appears to have been used for learning Git workflows and basic HTML.

## Current State

This is a nearly empty repository. Contents:

| File | Purpose |
|---|---|
| `Firsthtml.htm` | Basic HTML5 page — a simple landscape photo gallery template |
| `README.md` | Minimal project title only |
| `LICENSE` | MIT License (2019, Rahul Tushir) |

There is no Python code, no backend, no framework, and no build system.

## File Details

### `Firsthtml.htm`
A static HTML5 page with:
- A heading and paragraph referencing a landscape photo
- An `<img>` tag pointing to `photo.jpg` (file not present in repo)
- A link to the W3Schools HTML tags reference

```html
<!DOCTYPE html>
<html>
<head>
    <title>Page Title</title>
</head>
<body>
    <h1>A Photo of a Beautiful Landscape</h1>
    <a href="https://www.w3schools.com/tags">HTML tags</a>
    <p>Here is the photo123</p>
    <img src="photo.jpg" alt="Country Landscape">
</body>
</html>
```

## Development Workflows

### No build or run step required
This is a static HTML file. Open `Firsthtml.htm` directly in any browser to view it.

### Git Workflow
- The default branch is `master`
- Feature branches follow `claude/<description>` naming (e.g., `claude/add-claude-documentation-yJMij`)
- The project has had 2 pull requests merged historically

### No testing infrastructure
There are no tests, test runners, linters, or CI/CD pipelines configured.

## Conventions

Since there is no established code, the following are sensible defaults to follow if this project grows:

- **HTML**: Use HTML5 doctype, semantic elements, and include `alt` attributes on images
- **Python** (if added): Follow PEP 8 style, use a `requirements.txt` for dependencies
- **Commits**: Write clear, descriptive commit messages in imperative mood
- **Branches**: Create feature branches from `master`, use descriptive names

## Known Issues / Missing Pieces

- `photo.jpg` is referenced in `Firsthtml.htm` but not committed to the repository — the image will not render
- `README.md` contains only the project title; no description, setup, or usage instructions exist
- No `.gitignore` is present
- No Python code exists despite the repository name

## If You Are Adding Python Code

If this project is being expanded into an actual Python dashboard, recommended setup:

1. Add a `.gitignore` (include `__pycache__/`, `*.pyc`, `.env`, `venv/`)
2. Create a `requirements.txt` for dependencies
3. Add a `src/` or top-level module directory for application code
4. Set up a virtual environment before installing packages:
   ```bash
   python -m venv venv
   source venv/bin/activate   # Linux/macOS
   pip install -r requirements.txt
   ```
5. Update `README.md` with setup and run instructions
