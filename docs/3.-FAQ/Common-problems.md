

# Common problems 

**Jump to a Section:**

[TOC]

# Installing
These are the common problems while installing the released versions

## Common

## Windows

## Mac

## Linux

# Running
These are the common problems while running the released versions

## Common

### Final image has magenta elements
_TODO: reproduce and copy full errors_

#### Symptoms:
On completion of a blender task on the network the image shows magenta elements where it should not.

#### Description:
When the textures for rendering are missing it replaces them with these magenta elements. Please include all required texture files in the golem-task.

#### Resolution:
Check that you're using relative paths in your scene and that you have added all the required resources during task definition.

#### Found
unknown date by unknown

#### Relates to:
No issue reported

#### Affected version:
unknown

## Windows

### "Error Starting Docker" first run of golem after installation

#### Symptoms
- When `golem` starts it shows the error "Error Starting Docker"

image::https://user-images.githubusercontent.com/10008353/36040756-b3bc64ae-0dc6-11e8-84e4-08fa270300d9.png[Error starting docker]

#### Description
Docker requires specific settings to be able to run, check the included docker quickstart terminal for the full error and solve that first

#### Resolution
- close Golem
- hit windows key and type "Docker Quickstart Terminal"
- wait for it to start, this can take a while
- If any error appears, follow the proposed resolution

#### Found
20 Dec 2017 by @ederenn

#### Relates to:
None

#### Affected version:
None

### "Error Starting Docker" after upgrade of golem

#### Symptoms:
- When `golem` starts it shows the error "Error Starting Docker" 

image::https://user-images.githubusercontent.com/10008353/36040756-b3bc64ae-0dc6-11e8-84e4-08fa270300d9.png[Error starting docker]

- When starting `Docker Quickstart Terminal` it shows error "Error creating machine"

image::https://user-images.githubusercontent.com/10008353/36040768-bcba4b02-0dc6-11e8-829f-ff2bb13af2e9.png[Error creating machine]

- In `golem.log` it shows `ERROR    golem.docker.manager    DockerMachine: failed to start the VM: Command '['docker-machine', 'restart', 'golem']' returned non-zero exit status 1.`

#### Description:
During the upgrade of golem, VirtualBox also got updated, this caused the existing docker-machines to stop working. 

#### Resolution

- close Golem
- close VirtualBox in Task Manager
- hit windows key and type "Add or remove programs"
- then search for "virtual box" and select "modify"
- click modify -> repair
- restart

#### Found

20 Dec 2017 by @ederenn

#### Relates to

https://github.com/golemfactory/golem/issues/1786

#### Affected version

golem 0.9.1 and before

## Mac

## Linux

# Builds and tests

These are the common problems while running tests and building packages.

## Common
### Enum has Int field
_TODO: reproduce and copy full errors_

#### Symptoms:
`python setup.py develop` shows 
```
Enum has Int field
```

#### Description:
A dependency upgraded enum34 to a wrong version, please uninstall it.

#### Resolution:
Run with virtualenv enabled:
```
pip uninstall enum34
```

#### Found
unknown date by unknown

#### Relates to:
No issue reported

#### Affected version:
unknown

## Windows
### Import error: Twisted requires zope.interface
_TODO: reproduce and copy full errors_

#### Symptoms:
`pip install -r requirements.txt` shows 
```
Import error: Twisted requires zope.interface 3.6.0 or later: no module named zope.interface.
```

#### Description:
`zope.interface` was installed incorrectly. please re-install it with easy_install as non-admin user

#### Resolution:
Run in non-admin cmd with venv enabled:
```
easy_install zope.interface
```

#### Found
unknown date by unknown

#### Relates to:
No issue reported

#### Affected version:
unknown

### ImportError: No system module 'pywintypes'
_TODO: reproduce and copy full errors_

#### Symptoms:
`pip install -r requirements.txt` shows 
```
ImportError: No system module 'pywintypes' (pywintypes27.dll)
```

#### Description:
`pywin32` was installed incorrectly, it is missing a dll. please install the dll by downloading the correct version and adding it to the package or somewhere in the PATH

#### Resolution:
Download pywin32 https://sourceforge.net/projects/pywin32/files/pywin32/Build%20220/[from this site] install and copy `$PYTHON/Lib/site-packages/pywin32_system32/pywintypes36.dll` into `$PYTHON/Lib/site-packages/win32/`

or

Add `$PYTHON/Lib/site-packages/pypiwin32_system32` to the system PATH and restart your cmd

#### Found
- 23-nov-2017 by @maaktweluit during development of #1400
- Before 0.7.1 by unknown

#### Relates to:
No issue reported

#### Affected version:
external dependency

### EnvironmentError: Library "libgcc_s_dw2-1.dll" not found
_TODO: reproduce and copy full errors_

#### Symptoms:
When building in the mingw32 terminal `python setup.py develop` shows 
```
EnvironmentError: Library "libgcc_s_dw2-1.dll" not found
```

#### Description:
Your mingw32 installation is missing a required library, please download and add it manually.

#### Resolution:
Download the package gcc-core-4.4.0-mingw32-dll.tar.gz https://sourceforge.net/projects/mingw/files/MinGW/Base/gcc/Version4/Previous%20Release%20gcc-4.4.0/[from here]. Copy required dll from the bin folder into your mingw bin folder.

#### Found
unknown date by unknown

#### Relates to:
No issue reported

#### Affected version:
unknown

### ImportError: No module named win32api
_TODO: reproduce and copy full errors_

#### Symptoms:
When running `python setup.py develop` it shows 
```
ImportError: No module named win32api
```

#### Description:
pypiwin32 failed to install, try installing it without cache

#### Resolution:
Run this while your venv is loaded.
```
python -m pip install --no-cache pypiwin32
```

#### Found
unknown date by unknown

#### Relates to:
No issue reported

#### Affected version:
unknown

### Bad magic number in ...

#### Symptoms:
When running `python setup.py develop` it shows 
```
Bad magic number in ...
```

#### Description:
There is an error with your pyc files, please delete the and run again.

#### Resolution:
Run this in your golem source folder.
```
find . -name '*.pyc' -delete
```

#### Found
unknown date by unknown

#### Relates to:
No issue reported

#### Affected version:
unknown

### UnicodeDecodeError: 'utf-8' codec can't decode

#### Symptoms:
`pip install -r requirements.txt` shows 
```
Exception:
Traceback (most recent call last):
  File "c:\users\ederenn\projects\golem-env\lib\site-packages\pip\compat\__init__.py", line 73, in console_to_str
    return s.decode(sys.__stdout__.encoding)
UnicodeDecodeError: 'utf-8' codec can't decode byte 0xf1 in position 4: invalid continuation byte

During handling of the above exception, another exception occurred:

Traceback (most recent call last):
  File "c:\users\ederenn\projects\golem-env\lib\site-packages\pip\basecommand.py", line 215, in main
    status = self.run(options, args)
  File "c:\users\ederenn\projects\golem-env\lib\site-packages\pip\commands\install.py", line 342, in run
    prefix=options.prefix_path,
  File "c:\users\ederenn\projects\golem-env\lib\site-packages\pip\req\req_set.py", line 784, in install
    **kwargs
  File "c:\users\ederenn\projects\golem-env\lib\site-packages\pip\req\req_install.py", line 878, in install
    spinner=spinner,
  File "c:\users\ederenn\projects\golem-env\lib\site-packages\pip\utils\__init__.py", line 676, in call_subprocess
    line = console_to_str(proc.stdout.readline())
  File "c:\users\ederenn\projects\golem-env\lib\site-packages\pip\compat\__init__.py", line 75, in console_to_str
    return s.decode('utf_8')
UnicodeDecodeError: 'utf-8' codec can't decode byte 0xf1 in position 4: invalid continuation byte
```

#### Description:
You are missing the 'utf-8' codec on the python installation, you can edit your local pip as work-around

#### Resolution:
in `pip\compat\__init__.py:70` add this:
```
if sys.version_info >= (3,):
    def console_to_str(s):
        try:
            return s.decode(sys.__stdout__.encoding)
        except UnicodeDecodeError:
            try:
                return s.decode('utf_8')
            except UnicodeDecodeError:
                from ctypes import cdll
                os_encoding = 'cp' + str(cdll.kernel32.GetACP())
                return s.decode(os_encoding)
```

or

```
import locale
def console_to_str(s):
    return s.decode(locale.getpreferredencoding() or "utf-8", 'replace')
```

#### Found
29 November 2017 by @ederenn

#### Relates to:
https://github.com/golemfactory/golem/issues/1707

#### Affected version:
unknown

## Mac

## Linux


### ModuleNotFoundError: No module named 'setuptools'

#### Symptoms:
`python setup.py develop` shows 
```
Traceback (most recent call last):
  File "setup.py", line 5, in <module>
    from setuptools import setup
ModuleNotFoundError: No module named 'setuptools'
Error in sys.excepthook:
Traceback (most recent call last):
  File "/usr/lib/python3/dist-packages/apport_python_hook.py", line 63, in apport_excepthook
    from apport.fileutils import likely_packaged, get_recent_crashes
  File "/usr/lib/python3/dist-packages/apport/__init__.py", line 5, in <module>
    from apport.report import Report
  File "/usr/lib/python3/dist-packages/apport/report.py", line 30, in <module>
    import apport.fileutils
  File "/usr/lib/python3/dist-packages/apport/fileutils.py", line 23, in <module>
    from apport.packaging_impl import impl as packaging
  File "/usr/lib/python3/dist-packages/apport/packaging_impl.py", line 23, in <module>
    import apt
  File "/usr/lib/python3/dist-packages/apt/__init__.py", line 23, in <module>
    import apt_pkg
ModuleNotFoundError: No module named 'apt_pkg'

Original exception was:
Traceback (most recent call last):
  File "setup.py", line 5, in <module>
    from setuptools import setup
ModuleNotFoundError: No module named 'setuptools'
```

#### Description:
You are missing the python-dev package, it is required to run golem from source

#### Resolution:
Install python3.6-dev
```
sudo apt-get install python3.6-dev -y
```

#### Found
23 feb 2018 by @kascheri12

#### Relates to:
https://github.com/golemfactory/golem/issues/2184

#### Affected version:
All golem versions, commands are applicable from `0.12.0` ( python version upgrade )

### Building TaskCollector failed make: g++-5: Command not found
_TODO: reproduce and copy full errors_

#### Symptoms:
`setup.py develop` shows 
```
Building TaskCollector failed b'make: g++-5: Command not found\nmake: *** [Release/taskcollector] Error 127\n'
```

#### Description:
You are missing the `g\++-5` shortcut on your system library folder, you can link it to `g++`

#### Resolution:
```
sudo ln -s /usr/bin/g\+\+ /usr/bin/g\+\+-5
```

#### Found
unknown date by unknown

#### Relates to:
No issue reported

#### Affected version:
unknown

# Running source
These are the common problems when setting up and running from source

## Common

### argument --log-format: conflicting option
_TODO: reproduce and copy full errors_

#### Symptoms:
`pytest` shows 
```
argparse.ArgumentError: argument --log-format: conflicting option string(s): --log-format
```

#### Description:
Pytest and plugins are installed as an incorrect version, please re-install them from requirements-tst.txt

#### Resolution:
Clear your virtualenv and re install requirements.
```
python3 -m venv .venv --clear
pip install -r requirements.txt -r requirements-test.txt
```

#### Found
unknown date by unknown

#### Relates to:
No issue reported

#### Affected version:
unknown

## Windows

## Mac

## Linux

### SyntaxError: invalid syntax

#### Symptoms:
`python golemapp.py` shows 
```
Traceback (most recent call last):
  File "/usr/local/bin/golemapp", line 11, in <module>
    load_entry_point('golem', 'gui_scripts', 'golemapp')()
  File "/usr/local/lib/python3.5/dist-packages/pkg_resources/__init__.py", line 572, in load_entry_point
    return get_distribution(dist).load_entry_point(group, name)
  File "/usr/local/lib/python3.5/dist-packages/pkg_resources/__init__.py", line 2755, in load_entry_point
    return ep.load()
  File "/usr/local/lib/python3.5/dist-packages/pkg_resources/__init__.py", line 2408, in load
    return self.resolve()
  File "/usr/local/lib/python3.5/dist-packages/pkg_resources/__init__.py", line 2414, in resolve
    module = __import__(self.module_name, fromlist=['__name__'], level=0)
  File "/home/kentrendz/golem/golemapp.py", line 15, in <module>
    from golem.node import Node
  File "/home/kentrendz/golem/golem/node.py", line 4, in <module>
    from golem.client import Client
  File "/home/kentrendz/golem/golem/client.py", line 60, in <module>
    from golem.task.taskserver import TaskServer
  File "/home/kentrendz/golem/golem/task/taskserver.py", line 25, in <module>
    from .server import concent
  File "/home/kentrendz/golem/golem/task/server/concent.py", line 4, in <module>
    from golem.network.concent.handlers_library import library
  File "/home/kentrendz/golem/golem/network/concent/handlers_library.py", line 29
    self._handlers: typing.Dict[message.base.Message, weakref.ref] = {}
                  ^
SyntaxError: invalid syntax
```

#### Description:
The project switched to python 3.6 as lowest supported version, this error indicates python3.5 can not run the code anymore

#### Resolution:
Install python3.6 next to your system python ( do not replace it! )
```
sudo add-apt-repository ppa:jonathonf/python-3.6
sudo apt-get update && sudo apt-get install python3.6 python3.6-dev python3.6-venv -y
```
or
Build python 3.6 including dev and venv.

#### Found
22 feb 2018 by @kascheri12

#### Relates to:
https://github.com/golemfactory/golem/pull/2012

#### Affected version:
Last working version on 3.5 is 0.11.0, from 0.12.0 python3.6 is required

### EnvironmentError: Library "OpenEXR.so" not found
_TODO: reproduce and copy full errors_

#### Symptoms:
`golem.log` shows 
```
Library "OpenEXR.so" not found
```

#### Description:
You are missing the OpenEXR library in your system library folder, you can copy it from the installed python package to resolve this

#### Resolution:
```
sudo cp $HOME/.virtualenvs/golem-env/lib/python2.7/site-packages/OpenEXR.so /usr/lib/
```
or
Copy the OpenEXR.so from the Golem package

#### Found
unknown date by unknown

#### Relates to:
No issue reported

#### Affected version:
Pre python3, latest version 0.7.1

### EnvironmentError: Library "_psutil_linux.so" not found
_TODO: reproduce and copy full errors_

#### Symptoms:
`golem.log` shows 
```
EnvironmentError: Library "('_psutil_linux.x86_64-linux-gnu.so', '_psutil_linux.so', '/usr/local/lib/python2.7/dist-packages/psutil/_psutil_linux.so')" not found
```

#### Description:
You are missing the Process and system library in your system library folder.

#### Resolution:
Simplest way to fix this is to create a symlink:
```
sudo ln -s /usr/lib/python2.7/dist-packages/psutil /usr/local/lib/python2.7/dist-packages/psutil
```
and then
```
sudo ln -s /usr/local/lib/python2.7/dist-packages/psutil/_psutil_linux.x86_64-linux-gnu.so /usr/local/lib/python2.7/dist-packages/psutil/_psutil_posix.so
```

#### Found
unknown date by unknown

#### Relates to:
No issue reported

#### Affected version:
Pre python3, latest version 0.7.1
