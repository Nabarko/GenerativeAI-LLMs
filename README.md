![Python version](https://img.shields.io/badge/python-3.8-blue.svg)

# GenerativeAI-LLMs

--------
## Important

Please always create a separate environment for your project. There is a handy utility provided that could do
this for you, [read below](#make-init).

Please do not put confidential data useful for this project anywhere other than data folder.
The .gitignore is designed to ignore the folder contents making the project git safe.

Please keep your pyproject.toml and poetry.lock up to date with environments dependencies.
You can find more information about the [documentation and set up here](https://python-poetry.org/docs/).

If your project version supports a different python version, please change in the above badges along with
the pyproject.toml and Dockerfile.

Please remember to edit the pyproject.toml to suit your project. We are hoping to automate it as GitHub templates
allow for it in the future.


--------
## Actions

We are actively developing and maintaining Github Actions specifically for internal use in AstraZeneca.
 You can find the list of actions by
 [searching in AZ-AI org for repositories](https://github.com/AZ-AI?q=az-action&type=&language=&sort=)
 starting with az-action-.

There are some actions that run on this project by default:

1. Build Documentation
    - Build documentation for the project, ready for use with github pages
1. Version & Release
    - Use Semantic Versioning for your project. This relies on conventional commits, there is a check for this in the pre-commit hooks.



--------
## Project Organization


    ├── .github/workflows  <- Github actions.
    ├── Makefile           <- Makefile with utility commands.
    ├── Dockerfile         <- Create a Docker image for this project.
    ├── README.md          <- The top-level README for developers using this project.
    ├── data               <- The data folder for this project. This is always ignored by git by design.
    │  
    ├── docs               <- A default mkdocs project.
    │
    ├── models             <- Trained and serialized models, model predictions, or model summaries.
    │
    ├── notebooks          <- Jupyter notebooks. Please ensure the output is stripped out of any
    confidential information.
    │  
    ├── Dockerfile         <- A generic Dockerfile to help you get started.
    ├── generativeai_llms                <- Source code for use in this project.
    │

--------
## Set up Documentation Web Page

You can get your project documentation as a github website out of the box using this template.
To enable it you must:

1. Go to **Settings**.
1. Under the **Code and automation** header in the sidebar click **Pages**.
1. Under **Build and deployment** select **Deploy from a branch**
1. Choose **Branch** select **gh-pages**
1. Scroll to the bottom of the page and go to the url in the **Enforce HTTPS** section.

You should be able to view your documentation site! You can change the colours and some of the formatting in the `mkdocs.yaml` file.

--------
## Utilities Available:

### make init
Would create a pipenv environment for you along with pre-commit

### make clean
A utility tool to clear pycache and pyc or pyo files

If you find any issues or feature requests with the template, please [raise it here](https://github.com/AZ-AI/data-science-template)
