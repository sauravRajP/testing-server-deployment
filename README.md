# Testing-Server-Deployment

## 1. Create a github repo and download it to the local machine:
- Download repo: ``git clone <url>``
- Change directory to the cloned folder: ``cd <folder>``

## 2. Setup a django project:
- Create a virtual env: ``python3 -m venv env``
- Activate a virtual enironment: ``source env/bin/activate``
- Install django on virtual environment: ``pip install django``
- Create a django project: ``django-admin startproject <project_name>``
- Create a requirements.txt file: ``pip freeze > requirements.txt``

## 3. Ignore files from being tracked by Git:
- Create a .gitignore file with no extension.
- Ignore the virtual env files, cached files, files generated by IDE and settings.py file.
```python
env/
*.pyc
.vscode/
root_name/project_name/settings.py
```
- Add the files to github staging: ``git add .``
- Commit: ``git commit -m <commit -message>``

> Note: Every time changes is made to the file commit those files from the root directory.
