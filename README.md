![Python version](https://img.shields.io/badge/python-3.8-blue.svg)

# GenerativeAI-LLMs

--------
## Important

Please always create a separate environment for your project. There is a handy utility provided that could do
this for you, [read below](#make-init).

Please do not put confidential data useful for this project anywhere other than data folder.
The .gitignore is designed to ignore the folder contents making the project git safe.

--------
## Project Structure


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
