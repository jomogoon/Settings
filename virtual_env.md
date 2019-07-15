
# Python Virtualenv Setting
1. Install pip first
sudo apt-get install python3-pip

2. virtualenv
    sudo pip3 install virtualenv 
    virtualenv .env
    or 
    virtualenv --python=python3 .env

3. native
    sudo apt-get install python3.7-venv
    python -m venv .env
    source .env/bin/activate

4. activate
    Linux, Mac - source .env/bin/activate   
    Windows - .\.env\Scripts\activate

5. deactivate
deactivate

6. if required
    - map pip3 to pip
    - add alias to ~/.bashrc or ~/.bash_aliases
        alias python=python3
        alias pip=pip3

    - install with required.txt
    - pip install -U -r requirements.txt


# How to upgrade python
https://jcutrer.com/linux/upgrade-python37-ubuntu1810



# VS Code

C:\dev\projects\py\ChannelBreakoutBot\.vscode/settings.json
'''
{
    "python.pythonPath": ".env\\Scripts\\python.exe"
}
'''
