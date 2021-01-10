# lucabooks

1. Create environment in anaconda with python 3.7 and environment.yml

2. pip uninstall sphinxcontrib-bibtex

3. pip install sphinxcontrib-bibtex==1.0.0

4. Edit the following file: "_ init .py" (Anaconda3\envs\{env_name}\Lib\site-packages\jupyter_book\commands):
	- build_modified = max([os.stat(ii).st_mtime for ii in build_files]) (comment this out with #)
	- freshenv = True (set this to True)
5. Go to desired directory with 'cd'

6. jb create (name of your choiche)

7. jb build (same name as before)


in anaconda cmd:
- jupyter nbextension enable --py widgetsnbextension
- jupyter labextension install @jupyter-widgets/jupyterlab-manager
