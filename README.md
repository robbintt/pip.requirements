## Requirements Files

These are version pinned requirements files for various python virtualenvs.


### Purpose

Document what version I have been using.


### Maintenance

To maintain a requirements file:

1. Make a new environment and replace the relevant `requirements.txt`. 
2. Activate a virtualenv and upgrade everything; replace the relevant `requirements.txt`.
    - Upgrade individual packages manually or do a fresh pip install of the core dependencies
    - Upgrading is a major weakness of this way of doing things, most upgrade-all scripts are hackish
    - apparently `pip-tools` can upgrade all packages with `pip-compile --upgrade`


### System Setup

`mkdir ~/virtualenvs`
`ln -s /path/to/this/repo ~/virtualenvs/pip.requirements`

Then make whatever envs you need.


### How to

`pip freeze > virtualenv_name.txt`

Add comments to the top of this file.


### Template

Paste this into the top of the new requirements file and fill it out.

```
# Env: my-env-name
# OS: OS Version
# Date: YYYYMMDD
```

### Example

Don't use triple backticks when you paste this because they will cause issues in pip.

```
# Env: platformio
# OS:Ubuntu 16.04.2
# Date: 20170619
```

