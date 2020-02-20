# JupyterLab Installation

Assuming docker environment

## 1. Access docker
``` bash
$ sudo docker exec -it username /bin/bash
```

## 2. Update apt
``` bash
$ apt update
```

## 3. Install python3
currently only version 3.5 is available 
``` bash
 $ apt install python3
```
To download version 3.6, install from repo
``` bash
$ sudo add-apt-repository ppa:deadsnakes/ppa
$ sudo apt update
$ sudo apt install python3.6"
```

## 4. Install python pip
``` bash
 $ apt install python3-pip
```

## 5. Install vim
``` bash
 $ apt install vim
```

## 6. Install Jupyterlab
``` bash
 $ python3 -m pip install jupyterlab
```

## 7. Create Configuration File
``` bash
 $ jupyter notebook --generate-config
```
Writing default config to: /root/.jupyter/jupyter_notebook_config.py

## 8. Set jupyter lab password: ######
``` bash
 $ jupyter notebook password
```
>> creates this file: ~/.jupyter/jupyter_notebook_config.json

## 9. Copy sha1 to insert password into config file
``` bash
 $ vim ~/.jupyter/jupyter_notebook_config.json
```

## 10. Edit config file( ip address, port, folder, password)
``` bash
 $ vim ~/.jupyter/jupyter_notebook_config.py
```
Edit the following: (refer to vim manual)
- setting ip address: c.NotebookApp.ip = '210.117.119.55'
- setting port number: c.NotebookApp.port = 8888
- root directory setting: c.ContentsManager.root_dir = '/docker_data'
- c.NotebookApp.password = 'sha1:d2341...'

## 11. Starting Jupyter Lab Server
``` bash
 $ jupyter lab --no-browser --allow-root
```

In order to have the server running in the background:
``` bash
 $ jupyter lab --no-browser --allow-root &
```

## 12. List running jupyter server
``` bash
 $ ps -ef | grep jupyter
```

## 13. Kill jupyter server
``` bash
 $ sudo kill -9 PID
```

## 14. Install Python Packages
- Python Library 검색: https://pypi.org/ 

``` bash
 $ python3 -m pip install pandas
 $ python3 -m pip install --upgrade pandas
```
- to uninstall package
``` bash
 $ python3 -m pip uninstall pandas
```

## 15. Check version
``` bash
 $ python3 -m pip list install | grep pandas
```

## 16. Ouput Package Requirement text file
``` bash
 $ pip freeze > requirements.txt
```

