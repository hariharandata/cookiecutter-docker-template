# Cookiecutter docker template

In the context of a code repository, “cookie cutters” refer to project templates — standardized starting points used to generate new projects with a predefined structure, configuration, and boilerplate code.

This term typically comes from the Python project cookiecutter, a command-line utility that lets you create projects from templates. The idea is like a “cookie cutter” for code: you stamp out consistent project setups quickly.

⸻

🔧 What Is a Cookiecutter Repository?

A cookiecutter repo:
	•	Contains a project template directory (with Jinja2 templating syntax)
	•	Is structured to define file/folder names and contents dynamically
	•	Includes a cookiecutter.json file to prompt users for input (e.g., project name, author)



```markdown
my-docker-app/
├── Dockerfile
├── docker-compose.yml
├── pyproject.toml
├── ruff.toml
├── .env
├── README.md
├── src/
│   └── my_app/
│       └── main.py
├── tests/
│   └── test_main.py
```


When you run:
```markdown
cookiecutter https://github.com/yourorg/my-cookiecutter-template
```