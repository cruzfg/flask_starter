1. First create your virtual environment. If in Windows you can do this by running: gitbash_create_virtual_environment.sh.
   
   NOTE: that gitbash is a bash version written for Windows and not part of WSL.  It's intially easier to use than WSL. 

2. This first step will create a virtual environment named venv. Engineers call their virtual environment lots of different things but we will just call it venv by convention. 
   1. This is the convention I follow because venv is in the .gitignore file as it should be.

3. If in Windows GitBash OPEN the gitbash_activate.sh script because it doesn't work and copy paste it to the bash terminal in the VSCode editor and this should activate the venv you just created. 

4. Now that your venv is active install flask or if you already have a requirements.txt run that by using running: ./gitbash_install_requirements.sh otherwise run:
   1. python -m pip install flask
   
5. Since you are in your venv this will install flask or requirements.txt only in your venv.
   
6. This is the way we want to do installs only in the venv and keep your machine's python as clean as possible.

7. Now that you have installed flask or requirements.txt you have everything you need to create a web site using Model Template View pattern and/or everything you need to create a REST API.

8. You want to save this state especially if you are collaborating so you want to create a requirements.txt file. Run gitbash_create_requirements.sh. 
   1. If you have added packages to your project make sure you add via this script on step 8 or manually on the text file itself. See line item 10. 

9. You should see a requirements.txt file appear in your root directory.

10. If you are installing over pip packages, hold off on running the gitbash_create_requirements.sh script so that the pip packages you add on top installing flask can go into the requirements.txt file.

11. app.py is pointing to serve up the hello.html template out of the index view method. 

12. If you run the gitbash_dev_config_and_run_flask.sh you have your flask starter app running.

13. In gitbash all scripts are run ./<script_name>.sh [enter]

There is a few to do on the flask starter but the basics to get your flask app configured and running on both gitbash on Windows and bash on Linux or Mac is all done.

The gitbash_activate doesn't work yet but it's contents does. 

The linux_mac_activate is untested because I'm on windows and it's different than the gitbash_activate because the path to activate is different than on Linux or Mac. 

Why GitBash and not WML? I'm a Mac developer and my Mac was having trouble coming in. Having said that I had to get to work.  GitBash was an easy install on the Windows box and I didn't have time to read up on WML and files system mapping which I'm sure are simple enough but not simpler than installing GitBash and going. 

I'll have my Mac soon and test all the scripts on bash and figure out what's wrong with the activate script.  For now the work around to activate is easy enough.  And if you know venv then that script is just a helper script. 

