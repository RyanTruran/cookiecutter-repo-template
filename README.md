# cookiecutter-repo-template

## Getting Started

1. Click the "Use this template" button.
2. Update the `cookiecutter.json` with the required data.
3. Push the changes.

## What happens when the changes are pushed?

When the changes to the cookiecutter.json are pushed. The GitHub action will validate that the changes are not in a
template repo, then it will do the following.

1. Install cookiecutter
2. Execute cookiecutter, saving the output in a `cookiecutter-temp` directory
3. Removes all files that are not in the `cookiecutter-temp` directory.
4. Moves all files inside the `{{ cookiecutter.project_name }}` directory to the root directory.
5. Force pushes to the branch of the same name. 
