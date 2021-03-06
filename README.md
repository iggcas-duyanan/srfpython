# srfpython
  
- programs for surface wave dispersion curves in python
- compute, display, invert 1D depth models
- based on Herrmann codes Computer Program in seismology

install

> move to the installation path (e.g. "~/git") and get srfpython
>
> ```
> cd ~/git
> git clone http://github.com/obsmax/srfpython.git
> ```
>
> create the virtual environment and activate it
>
> ```
> conda create -n srfpython python=2.7
> source activate srfpython
> ```
>
> move to the repository, install the requirements and install the package
>
> ```
> cd ~/git/srfpython
> conda install --yes --file requirements.txt
> pip install -e .
> ```
>
> compile fortran codes
>
> ```
> cd ~/git/srfpython/srfpython/Herrmann/src90
> ./clean.sh 
> ./compile.sh
> ```
>
> test fortran codes using
>
> ```
> python ~/git/srfpython/srfpython/Herrmann/Herrmann.py
> ```

add the bin directory to the path (recommended)

> custom the following line and add it to
> your .bashrc or .bash_path (linux) or .profile (mac)
>
> ```
> export PATH=$PATH:"~/git/srfpython/srfpython/bin"
> ```

if you plan to use jupyter notebooks with python2 (optional)

> make sure the environment is activated
> ```
> source activate srfpython
> ```
>
> install with
>
> ```
> conda install --yes notebook ipykernel
> ipython kernel install --user
> ```
>

try the tutorials

> ```
> cd ~/git/srfpython/tutorials/tutorial0
> jupyter notebook 
> ```
