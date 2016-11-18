venv_pip_installer
==================

Deploy pip packages in Virtualenv with optional apt packages dependencies



Role Variables
--------------

Mandatory variables:

    - venv_path  : Virtualenv Root Path
    - venv_python  : python binary (ex: python3.5)
    - venv_pip_packages : List of pip packages to deploy


Optionnal vars:
    - venv_apt_dependencies : list of apt packages to deploy before pip install
    - venv_pip_extra_args : extra arg send to pip while install


How to use 
----------

    - hosts: server
      roles:
         - { role: venv_pip_installer, venv_path: "/oscaro/venv", venv_python: "python3.5", venv_pip_packages: [uwsgi, django,myapp] }


License
-------

Licensed under the MIT License. See the [LICENSE](LICENSE) file for details.


Author Information
------------------
Benjamin Jolivot
bjolivot@gmail.com
See my other "work on my computer" ansible things on https://www.github.com/bjolivot
