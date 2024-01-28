# Calmcode 1

## Virtual Environments

1. The first step was installing 2 different versions of python and adding them to the **PATH**. I have gone with python 3.7 and python 3.12 versions.

2. Installing virtualenv
	 - Installing virtualenv compatible with 3.7 with the command <br>
	   `
            python -m pip install virtualenv
           `
	- Installing virtualenv compatible with 3.12 with the command <br>
          `
          python3 -m pip install virtaulenv
          `
               
3. Creating virtualenv for each of the python versions
	- Creating virtualenv for version 3.7 (venv37) and activating it<br>
			```# Create virtualenv```<br>
			```python -m virtualenv venv37``` <br> 
			```# Activate venv37``` <br>
			```.\venv37\Scripts\activate```<br>
			```# Check python version:``` <br>
			```python --version```  <br>
	- Creating virtualenv for version 3.12 (venv312) and activating it<br>
		```# Create virtualenv```<br>
		``` python3 -m virtualenv venv312```<br>
		``` # Activate venv312```<br>
		```.\venv312\Scripts\activate```<br>
		```# Check python version```<br>
		``` python --version```<br>

4. Installing Packages
	- For venv37, I have manually installed packages by directly running pip install command in the terminal after which I checked current packages<br>
```# Check current packages```<br>
```pip freeze # this gives us no packages as its a new virtualenv```<br>
```# Install pandas and fastapi```<br>
```pip install pandas fastapi```<br>
```# Verify that the packages are installed```<br>
```pip freeze # Result shows pandas and fastapi are installed```<br>

	- For venv312, I have used requirements312.txt to install the python packages. This file contains the exact pinned versions of the packages I want to install.<br>
```# Check current packages```<br>
```pip freeze # No packages installed currently```<br>
```# Run pip install using requirements312.txt```<br>
```pip install -r requirements312.txt```<br>
```# Checking for installed packages```<br>
```pip freeze```<br>
