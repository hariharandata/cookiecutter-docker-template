# Cookiecutter docker template

In the context of a code repository, “cookie cutters” refer to project templates — standardized starting points used to generate new projects with a predefined structure, configuration, and boilerplate code.

This term typically comes from the Python project cookiecutter, a command-line utility that lets you create projects from templates. The idea is like a “cookie cutter” for code: you stamp out consistent project setups quickly.

A Cookiecutter template to scaffold Docker-based projects with a standardized structure, facilitating rapid development and deployment.

⸻

## 🔧 What Is a Cookiecutter Repository?

A cookiecutter repo:
- Contains a project template directory (with Jinja2 templating syntax)
- Is structured to define file/folder names and contents dynamically
- Includes a cookiecutter.json file to prompt users for input (e.g., project name, author)


## Features
- Predefined directory structure for Docker-centric applications
- Customizable project attributes via Cookiecutter prompts
- Includes essential configuration files: Dockerfile, .dockerignore, and README.md
- Supports integration with CI/CD pipelines
- Lightweight and adaptable to various project types


## Requirements
- [Cookiecutter](https://cookiecutter.readthedocs.io/en/latest/installation.html)
- [Docker](https://www.docker.com/get-started)



## Quickstart
1.	Install Cookiecutter:

```bash
pip install cookiecutter
```
2.	Generate a new project:
```bash
cookiecutter https://github.com/hariharandata/cookiecutter-docker-template.git
```


3.	Provide the required information when prompted:
- project_name: Your project’s name
- project_slug: Directory name for the project
- description: A brief description of the project
- author_name: Your name
- python_version: Python version to use (e.g., 3.8)

4.	Navigate to your new project directory:
```bash
cd your_project_slug
```
5.	Build and run your Docker container:
```bash
docker build -t your_project_slug .
docker run -it your_project_slug
```

## Project Structure
```markdown
your_project_slug/
├── .dockerignore
├── Dockerfile
├── README.md
├── app/
│   └── main.py
└── requirements.txt
```

- app/main.py: Entry point of your application
- requirements.txt: Python dependencies
- Dockerfile: Instructions to build the Docker image
- .dockerignore: Specifies files and directories to ignore when building the image


## Customization

Feel free to modify the generated files to suit your project’s specific needs. For example:
- Add more Python modules in the app/ directory
- Update requirements.txt with additional dependencies
- Enhance the Dockerfile with environment variables or additional setup steps

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your enhancements.

## License
This project is licensed under the MIT License.


