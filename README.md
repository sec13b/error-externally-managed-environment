
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
× This environment is externally managed
╰─> To install Python packages system-wide, try apt install
    python3-xyz, where xyz is the package you are trying to
    install.
    
    If you wish to install a non-Debian-packaged Python package,
    create a virtual environment using python3 -m venv path/to/venv.
    Then use path/to/venv/bin/python and path/to/venv/bin/pip. Make
    sure you have python3-full installed.
    
    If you wish to install a non-Debian packaged Python application,
    it may be easiest to use pipx install xyz, which will manage a
    virtual environment for you. Make sure you have pipx installed.
    
    See /usr/share/doc/python3.11/README.venv for more information.

note: If you believe this is a mistake, please contact your Python installation or OS distribution provider. You can override this, at the risk of breaking your Python installation or OS, by passing --break-system-packages.
hint: See PEP 668 for the detailed specification.
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
1. find /usr/lib -name EXTERNALLY-MANAGED
2.sudo mv /usr/lib/python3.11/EXTERNALLY-MANAGED /etc/motd
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~



here's mine opinion
Issue: You're trying to install a Python package using pip, but the environment is externally managed, meaning that package management is handled by the system package manager (apt) rather than pip.

Suggested Solutions:
1. Install system-wide using apt: Try installing the package using apt, like this: apt install python3-xyz, replacing xyz with the package name you're trying to install.

2. Create a virtual environment: Create a virtual environment using python3 -m venv path/to/venv, then activate it and install packages using pip.

3. Use pipx: If you want to install a non-Debian-packaged Python application, consider using pipx install xyz, which will manage a virtual environment for you.
