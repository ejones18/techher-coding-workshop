# Downloading and setting up your Python environment

## Installing the latest, supported Visual C++ Redistributable packages.

Before we get started with installing Python, we need to install the latest C++ redistributable packages! To do this, visit https://docs.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist?view=msvc-170#visual-studio-2015-2017-2019-and-2022 and download the relevant package as per the list below:

* Windows 11 - X64 package

* MacOS - ARM64 package

* Windows 10 - Check your system architecture by opening a Command Prompt instance and running the command ```echo %PROCESSOR_ARCHITECTURE%```. If the result of that is ```X86``` then download the X86 package or if the result is ```AMD64``` then download the X64 package!

Once that has been downloaded, click on the downloaded file and follow the installation wizard to the end - *you may require a system restart which is totally fine!*

## Downloading Python to your machine

For this workshop we'll be using Python3.7.7, however any version over Python3.5 is perfectly fine! You'll need to navigate over to https://www.python.org/downloads/release/python-377/ and download the following installer depending on your operating system:

* WindowsOS - MD5 sum #e0c910087459df78d827eb1554489663

* MacOS - MD5 sum #47b06433e242c8eb848e035965a860ac

You can find short videos of the installation process for each of the operating systems below:

* WindowsOS - https://www.youtube.com/watch?v=VWgs_iTojoA

* MacOS - https://www.youtube.com/watch?v=X5iTd5vT0Ns&t=171s

**Note - Ensure you you click the tick box that 'Adds Python to your environment (PATH) variables' during the installation! Other than that, install with the defualt settings**

Now that you have Python installed on your own machine, you can run the command ```python --version``` in a brand new terminal/powershell/console instance to check the version you have installed.

## Setting up your environment

As for the teaching materials for to this workshop, we'll be using Jupyter Notebooks - these are interactive journals that streamline any set-up.

### Cloning the respository

First you'll need to clone the Github repository, but to do this you'll need to install git in a similar way we installed Python. 

Navigate over to the page here https://git-scm.com/downloads and select your operating system to download. Once this has installed, again by following the installation wizard accepting all the default settings, navigate to a brand new terminal/powershell/console window and type ```git``` - this should print the git helper to your screen!

To clone the repository, you'll want to type in the command ```git clone https://github.com/ejones18/techher-coding-workshop.git```in a terminal/powershell/console instance which will bring all the workshop material onto your own machine!

**Note A: This will open up a small authentication window, click on the `sign in in browser` option and then sign into GitHub to continue!**

**Note B: be sure to remember the path to the folder where the content has been cloned to!**

### Installing the packages

To begin with, we'll need to update the pip package manager! This can be done by running the command ```python -m pip install --upgrade pip``` in the  terminal/powershell/console instance you have open!

To install the packages required for this workshop, run the command ```pip install -r "requirements.txt"``` in a terminal instance within Visual Studio Code, *after you've opened up the folder you've just cloned*. This may take a few minutes due to packages we are using so don't worry if it takes a bit of time!

## Using Visual Studio Code with the learning material - suggested

Now that everything is installed and ready for use, let's look at how we actually use it! 

First off, you'll want to open the `intro-to-python-workshop` folder in Visual Studio (VS) Code - if you haven't done so already. As we've installed the Juypter extension we can view the notebooks within our VS Code IDE! If you open up the first notebook of this module, in order to run the cell you will be prompted for a `kernal` at the top right of the page - at this stage be sure to select the python3.7.7 kernal as this will have all the packages installed! Now you should be able to go about the learning material - should you be prompted for a kernal on another notebook, select the same one as before!

From here you can run each of the cells from all the notebooks - happy learning!

## Using your browser to access the learning material

If prefered, participants can use their browser to interactive with the notebook content - this may allow them to utilise immersive reader extensions to aid them in reading. To do this open a new instance of terminal/powershell/console (within VS Code when you've opened the folder we cloned) and then run the command `jupyter notebook` and then wait for it to load up in your browser!

This creates a Jupyter server for you to access the content through your web browser - to shut the server down, in the terminal where you run the previous hit `ctrl+C` until the server shuts down.

Happy coding!
