# Calmcode 1

## Virtual Environments

1. The first step was installing 2 different versions of python and adding them to the **PATH**. I have gone with python 3.7 and python 3.12 versions.

2. Installing virtualenv
	 - Installing virtualenv compatible with 3.7 with the command 
		```python -m pip install virtualenv```

	- Installing virtualenv compatible with 3.12 with the command
      ```python3 -m pip install virtaulenv```
      
3. Creating virtualenv for each of the python versions
	- Creating virtualenv for version 3.7 (venv37) and activating it
			```# Create virtualenv```
			```python -m virtualenv venv37```  
			```# Activate venv37``` 
			```.\venv37\Scripts\activate```
			```# Check python version:``` 
			```python --version```  
	- Creating virtualenv for version 3.12 (venv312) and activating it
		```# Create virtualenv```
		``` python3 -m virtualenv venv312```
		``` # Activate venv312```
		```.\venv312\Scripts\activate```
		```# Check python version```
		``` python --version```

4. Installing Packages
	- For venv37, I have manually installed packages by directly running pip install command in the terminal after which I checked current packages
```# Check current packages```
```pip freeze # this gives us no packages as its a new virtualenv```
```# Install pandas and fastapi```
```pip install pandas fastapi```
``` #Verify that the packages are installed```
```pip freeze # Result shows pandas and fastapi are installed```

	- For venv312, I have used requirements312.txt to install the python packages. This file contains the exact pinned versions of the packages I want to install.
```# Check current packages```
```pip freeze # No packages installed currently```.
```# Run pip install using requirements312.txt```
```pip install -r requirements312.txt```
```# Checking for installed packages```
```pip freeze```
