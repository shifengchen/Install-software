#   [Install pip](https://pip.pypa.io/en/stable/installing/)

## [Use Virtual Environments](http://docs.python-guide.org/en/latest/dev/virtualenvs/)

```bash
// Install virtualenv via pip
pip install virtualenv

// Test your installation
virtualenv --version
```

### Basic Usage
1.Create a virtual environment for a project:
```bash
cd my_project_folder
virtualenv venv
```

2.To begin using the virtual environment, it needs to be activated:
```bash
source venv/bin/activate
```

3.If you are done working in the virtual environment for the moment, you can deactivate it:
```bash
deactivate
```

### Other Notes
```bash
pip freeze > requirements.txt

pip install -r requirements.txt
```
