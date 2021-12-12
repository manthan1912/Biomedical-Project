# Predicting Synergistic Drug Combinations using Machine Learning Techniques.

#### Abstract:
Breast cancer is a disease in which the cells in the breast split out of control. It is a major health problem worldwide principally among women and this cancer may spread to other parts of the body in most cases. This cancer is observed in the age group of 25 – 50. On average, 75 women are being diagnosed with breast cancer every day in Canada and 14 women die each day. Though the survival chances of vary based on the stage of cancer and patient’s response to the treatment, chemotherapy is used as a main treatment in majority of situations. Cancers cells are known to develop resistance to targeting drugs over the course of treatment and this leads to cancer recurrence. To overcome this problem, it is essential to implement drug combination therapy, where two or more drugs combined to target the cancer which delays the resistance of cancer over the drugs and decreases toxicity. Whenever a new drug is invented, the chances to identify a new drug combination reduce. Advancement in the field of computer science and biology, lead to an evolution of ‘bioinformatics’. Application of machine learning to this field optimized the problem of discovering new drug combination to cure cancers. In this paper, we aim to predict new drug combinations, through machine learning methods, that can be effective in breast cancer treatment.

#
Steps:
1) Download Anaconda.
2) Install Anaconda in your system.
3) Install rdkit environment in conda.
4) Open Anaconda Navigator
5) Open Jupyter Notebook from the Anaconda Navigator


# Download Anaconda3-2021.11

Anaconda is a python and R distribution. It aims to provide everything you need (Python-wise) for data science "out of the box".
Download it from [here](https://www.anaconda.com/products/individual)

* Note: We need Conda environment to run rdkit module.


## Installing Anaconda
After downloading the software, 
* Double click on it to start the installation process.
* Click Next.
* Read the licensing terms and click “I Agree”.
* Select an install for “Just Me” unless you’re installing for all users (which requires Windows Administrator privileges) and click Next.
*  Select a destination folder to install Anaconda and click the Next button.
* ![](https://docs.anaconda.com/_images/win-install-destination.png)

* It is recommended to not tick the "Add Anaconda3 to my Path". 
* Instead use Anaconda software by opening Anaconda Navigator or the Anaconda Prompt from the Start Menu.
![../../../_images/win-install-options.png](https://docs.anaconda.com/_images/win-install-options.png)

*  Click the Install button. If you want to watch the packages Anaconda is installing, click Show Details.
* Click the Next button.
* This is optional. Install Anaconda without PyCharm, click the Next button.![../../../_images/win-install-pycharm.png](https://docs.anaconda.com/_images/win-install-pycharm.png)

* After a successful installation you will see the “Thanks for installing Anaconda” dialog box:
![../../../_images/win-install-complete.png](https://docs.anaconda.com/_images/win-install-complete.png)

** For MacOs **  Check https://docs.anaconda.com/anaconda/install/mac-os/

### After succesfull installation of the Anaconda software, click on Start Menu and search for "Anaconda Navigator".

* Anaconda Navigator is a desktop graphical user interface (GUI) included in Anaconda® distribution that allows you to launch applications and easily manage conda packages, environments, and channels without using command-line commands. Navigator can search for packages on Anaconda.org or in a local Anaconda Repository. It is available for Windows, macOS, and Linux.
![../../_images/nav-defaults.png](https://docs.anaconda.com/_images/nav-defaults.png)

* Next step is to install rdkit environment in Conda. 
* To do that click on  **CMD.exe Prompt**  inside the Anaconda Navigator.
* A command prompt will appear. Type the following command
	```bash
	(base) C:\Users\{username}> conda create -c conda-forge -n my-rdkit-env rdkit
	```
* ```bash
	Proceed ([y]/n)? y *press y and enter*
```
* Once the installation of the rdkit environment is complete you will see 
```bash
Preparing transaction: done
Verifying transaction: done
Executing transaction: done
To activate this environment, use
$ conda activate my-rdkit-env
To deactivate an active environment, use
$ conda deactivate 
```
* Next, we activate the environment.
``` bash
> conda activate my-rdkit-env
```
* Once you are inside the rdkit environment you will see (base) changed to (my-rdkit-env)
```bash
(my-rdkit-env) C:\ Users\ username >
```

* Now we install **XGBoost** module in rdkit conda environment.
* To do so, type pip install xgboost in the command prompt of anaconda
 ``` bash
pip install xgboost 
 ```

* Next we install sklearn:
 ``` bash
pip install sklearn 
 ```
* Install Seaborn:
 ``` bash
pip install seaborn 
 ```

Other packages such as
1) Pandas
2) Numpy
3) Matplotlib

are already installed while installing the conda environment.

### Now, Go to Anaconda Navigator, click on "Applications on" dropdown and select "my-rdkit-env".

*  Since we have installed a new environment, we need to install the jupyter notebook for this environment.
* Hence, click on install under "Jupyter Notebook" box.
* Once the installation is done, the "install" button will be changed into "Launch".
* Just click on launch and the browser window will open with the default jupyter location.
* Open the folder where the project files are stored.
* First, open the "preprocessing_and_dataset_preparation.ipynb" file.
* Then run the "modelling_and_results.ipynb".

