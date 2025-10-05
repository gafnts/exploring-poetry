# Exploring Poetry

This repository is a simple and opinionated demonstration of using [Poetry](https://python-poetry.org/) for Python project management. Along with some thoughts and best practices.

## Why I stopped using conda: the case for project-local environments

When you first learn it, Conda seems to "abstract the complexity away". I'm here to tell you, it doesn't, it just moves it somewhere else, awaiting you to deal with it later. And sooner than later, oh, you will have to deal with it.

Conda environments living in some central location instead of `.venv` in your project folder is *maddening*. It breaks so many workflows:

- You can't just delete the project folder and have everything gone: you've got this orphaned environment somewhere
- It is harder to version control settings: the environment isn't obviously tied to the project
- It is confusing for other developers: "which environment goes with which project again?"
- It breaks a simple mental model: the project and its dependencies should be together

