# stock-explorer
Small package to automatically download stock data and perform some basic exploration

## Project Settings
This project contains a great deal of user defined settings which are captured in the [settings file](settings.yml).  
Please review.

## Execution
This repo is executed in a Jupyter [Notebook](explorer.ipynb).  If you are unfamiliar with Jupyter please see this [site](https://jupyter-notebook-beginner-guide.readthedocs.io/en/latest/what_is_jupyter.html).  

The following instructions are written for a Windows environment but should be extremely similar for Linux or OS X.

1. Clone repo to PC.  If you don't have git installed, you can get it [here](https://git-scm.com/).
   ```shell script
   git clone https://github.com/daniel-fudge/stock-explorer.git
   ```

1. Install [Anaconda3](https://www.anaconda.com/distribution/).

1. Create a virtual environment.  Please see this [site](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html) 
for more conda environment information.
   ```shell script
   conda update conda
   conda create -n explorer
   conda activate explorer 
   conda install ipykernel
   conda install jupyter
   conda install matplotlib
   conda install pandas
   conda install pandas-datareader
   conda install pyyaml
   conda install scikit-learn
   conda install seaborn
   ipython kernel install --name=explorer
   pip install alpha_vantage
   ```
   
1. Activate the virtual environment if not already activated.  Note the above steps only need to be executed once.  
After initial setup you can start at this step.
   ```shell script
   conda activate explorer
   ```

1. Launch Jupyter.
   ```shell script
   cd stock-explorer
   jupyter notebook
   ```

1. Open the [notebook](explorer.ipynb).

1. Read and/or run the cells at your leisure!!  :)

## License
This code is copyright under the [MIT License](LICENSE).

## Contributions
Please feel free to raise issues against this repo if you have any questions or suggestions for improvement.
