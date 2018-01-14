# machine learning exercises

## requirements

* python
* pip
* jupyter-notebooks

## how to run

1. create a virtual environment

	$ python -m venv venv

2. activate the environment

	$ source ./venv/bin/activate

3. install dependencies

	1. pytorch

		$ pip3 install http://download.pytorch.org/whl/cu80/torch-0.3.0.post4-cp36-cp36m-linux_x86_64.whl

	2. other requirements:

		$ pip -r requirements

4. create python kernel

	$ python -m ipykernel install --user --name <venv-kernel-name>

5. run the notebook (opens in browser)

	$ jupyter notebook

	in the browser window go to the "Kernel" menu and select the kernel <venv-kernel-name>
	navigate to "src/....ipynb" and the notebook will show up

6. deactivate environment

	$ deactivate

## how to keep the repository clean

install [nbstripout](https://github.com/kynan/nbstripout):

	$ source ./venv/bin/activate    # activate environment
	$ pip install nbstripout nbconvert

activate it:

	$ nbstripout --install

This enables a filter in the git repository, which hides the cell outputs from git.
This way cell output is not added to the repo.

NICE!
