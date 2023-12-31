# {{cookiecutter.project_name}}

This is a simple application for NAO (or Pepper with NAOqi 2.5).

It consists of a Python 3 script (`app/scripts/main.py`) wrapped in a Choregraphe project, in such a way that the choregraph application is running if and only if the python script is running.

It requires the package with Python 3 for NAO to be installed on the robot.

## Running it on NAO

Open the project (select `app/{{cookiecutter.project_slug}}.pml`) with Choregraphe, then you can install it normally launch it from there (or add trigger conditions etc.)


## Running it from your computer

During development, it might be more convenient to run the script from your computer.

You will need a Python 3 environment with [libqi for Python](https://pypi.org/project/qi/) installed; in which case you can run

> python3 app/scripts/main.py --qi-url <your robot's IP address>

Initially generated by cookiecutter from http://github.com/EmileKroeger/cookiecutter_naoapp