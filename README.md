# wolfram-jupyter
Use this to run the Wolfram Engine locally through a Jupyter Notebook.

# Installation

## Mac/UNIX

### Prerequisites

* **Jupyter**: Can be installed through Anaconda or with `brew install jupyter` from the command line if you have Homebrew installed. To check if you have it installed correctly, try launching it with e.g. `jupyter notebook` in the command line.

For the next two prerequisites, you need a Wolfram account. If you do not have one already, you can create one at https://account.wolfram.com/login/create. You should also verify your e-mail.

* **Wolfram Engine**: Download the free Wolfram Engine at https://www.wolfram.com/engine/, choosing the download that corresponds to your system. On mac, run the .dmg file and double click the download manager that appears in order to start the installation. After installation you need to activate the free license that comes with the product. To do so, simply run the Wolfram Kernel.


* **wolframscript**: To install wolframscript, follow the guide at https://reference.wolfram.com/language/workflow/InstallWolframScript.html. Again, you must activate the free license by running `wolframscript` in the command line after installation. _Note_: To avoid some known problems, you should make sure to install and activate the Wolfram Engine before wolframscript.

### Linking Wolfram Engine to Jupyter
Go to a suitable folder and clone the repository

`` git clone https://github.com/WolframResearch/WolframLanguageForJupyter.git `` 

Enter the directory `WolframLanguageForJupyter` and run the configuration script 

`` ./configure-jupyter.wls add ``

Note: If your Wolfram Engine path should ever change, you need to run the configuration script again.

## Windows


# Running
You can run the Wolfram Kernel through either Jupyter Labs or Jupyter Notebooks. Choose the one you prefer and launch it with

`` jupyter notebook `` or `` jupyter lab``

in the command line. This should open a browser window. If you chose Notebooks, you can create a new notebook by pressing the "new" button in the top right corner of the UI; there, you should see the Wolfram Kernel as an option for the kernel you want to run the notebook on (instead of, e.g., Python). If you chose labs, you should see a Wolfram Kernel icon under the "Notebooks" category when creating a new project.

When in your Wolfram Kernel notebook, you can execute Mathematica commands like `Plot[Hypergeometric2F1[3/4, 1, 5/4, -1/x^2],{x,0,10},PlotTheme->"Detailed"]` and `Integrate[q^2/(Exp[q]+1),{q,0,Infinity}]` by writing them in a cell and executing the cell by pressing `shift + enter`. The advantage in running through a notebook is the neat inherent workflow of notebooks and the availability of the graphics (contrary to simply running wolframscript through the command line).

For example notebooks showcasing basic Mathematica usage, refer to the notebooks in this repository.

# License notes
