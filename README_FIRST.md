# Data Science in VS Code tutorial
This tutorial demonstrates using Visual Studio Code and the Microsoft Python extension with common data <br>
science libraries to explore a basic data science scenario. Specifically, using passenger data from the Titanic, <br>
you will learn how to set up a data science environment, import and clean data, create a machine learning model <br>
for predicting survival on the Titanic, and evaluate the accuracy of the generated model.

## <b>Prerequisites</b>
The following installations are required for the completion of this tutorial. Make sure to install them if you <br>
haven't already.<br>

- [VS Code](https://code.visualstudio.com/)
- [Python extension](https://marketplace.visualstudio.com/items?itemName=ms-python.python) for VS Code
- [Jupyter extension](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter) for VS Code
- [Miniconda](https://docs.anaconda.com/miniconda/) with latest Python

    ><b>Note:</b> If you already have the full <b>Anaconda distribution</b> installed, you don't need to install <br>
    ><b>Miniconda</b>. Alternatively, If you'd prefer not to use Anaconda of Miniconda, you can create a <br>
    ><b>Python virtual environment</b> and install the packages needed for the tutorial using pip. If you go <br>
    >this route, you will need to install the following packages:
    >- pandas
    >- jupyter
    >- seaborn
    >- scikit-learn
    >- keras
    >- tensorflow

## <b>Set up a data science environment</b>
Visual Studio Code and the Python extension provide a great editor for data science scenarios. With native <br>
support for Jupyter notebooks combined with Anaconda, it's easy to get started. In this section, you will <br>
create a workspace for the tutorial, create an Anaconda environment with the data science modules needed <br>
for the tutorial, and create a Jupyter notebook that you'll use for creating a machine learning model.

1. Begin by creating an Anaconda environment for the data science tutorial. Open an Anaconda <br>
    command prompt and run `conda create -n myenv python pandas jupyter seaborn scikit-learn keras tensorflow` <br>
    to create an environment named <b>myenv</b>. For additional information about <br>
    creating and managing Anaconda environments, see the [Anaconda documentation](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html).

2. Next, create a folder in a convenient location to serve as your VS Code workspace for the tutorial, name <br>
    it `hello_ds`.

3. Open the project folder in VS Code by running VS Code and using the <b>File > Open Folder</b> command.
    You can safely trust opening the folder, since you created it.

4. Once VS Code launches, create the Jupyter notebook that will be used for the tutorial. Open the
    command Palette (`Ctrl+Shift+P`) and select <b>Create: New Jupyter Notebook</b>.

    ![alt text](image.png)
    > <b>Note:</b> Alternatively, from the VS Code File Explorer, you can use the New File icon to create a <br>
    > Notebook file named `hello.ipynb`

5. Save the file as `hello.ipynb` using <b>File > Save As...</b>

6. After your file is created, you should see the open [Jupyter notebook](https://jupyter.org/) in the notebook editor. <br>
    For additional information about native Jupyter notebook support, you can read the [Jupyter Notebooks](https://code.visualstudio.com/docs/datascience/jupyter-notebooks) topic.

    ![alt text](image-1.png)

7. Now select <b>Select Kernel</b> at the top right of the notebook.
    ![alt text](image-2.png)

8. Choose the Python environment you created above in which to run your kernel.
    ![alt text](image-3.png)

9. If your environment is not activated, you can do so as you would in your terminal (Anaconda command prompt) <br>
    `conda activate myenv`.

## Prepare the data
Please refer to the Jupyter notebook file named `hello.ipynb` for further details