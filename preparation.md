# Preparation

## Format

The tutorial consists of lecture segments, followed by hands-on
exercises.  We strongly encourage you to bring a laptop with all the
required packages installed in order to participate fully.

## Software required
- Python

  If you are new to Python, please install the
  [Anaconda distribution](https://www.anaconda.com/distribution/) for
  **Python version 3** (available on OSX, Linux, and Windows).
  You will also need to install [napari](https://napari.org), using
  either `pip install napari` or `conda install -c conda-forge napari`.
  Make sure you execute those commands in the appropriate environment. If you
  are not sure what that means, it might be a good idea to come early to the
  session to ask the organisers for help.
  
- Git (optional)
  Please install Git if you don't already have it on your computer.
  Here is how you can install Git on different Operating Systems https://github.com/git-guides/install-git
  
## Download lecture material


### Option 1: using git

If you are familiar with git, you can clone the repository at
https://github.com/jni/skimage-tutorials.

```
git clone --depth 1 https://github.com/jni/skimage-tutorials
git checkout --track origin/monash-df-2020-08
```

We may make editorial corrections to the material until the day before
the workshop, so please execute `git pull` to update before class.

### Option 2: download a zip file

Download the file at:

https://github.com/jni/skimage-tutorials/archive/monash-df-2020-08.zip

Unzip it, then start a jupyter notebook inside the archive.

# Tools and Python Packages
  If you are comfortable with environments, feel free to use your favorite
  distribution, but please ensure the requirements below are met:

  - scikit-image >= 0.17
  - numpy >= 1.12
  - scipy >= 1.0
  - matplotlib >= 2.1
  - notebook >= 4.0
  - scikit-learn >= 0.18
  - pandas >= 0.25
  - napari >= 0.3

  We have provided a conda environment that should work well for the workshop,
  see `environment.yml`. You can create it with:

  ```bash
  cd skimage-tutorials
  conda env create -f environment.yml
  conda activate skimage-tutorial
  ```

  Please see "Test your setup" below.

- Jupyter

  The lecture material includes Jupyter notebooks.  Please follow the
  [Jupyter installation instructions](http://jupyter.readthedocs.io/en/latest/install.html),
  and ensure you have version 4 or later and notebook version 6 or later:

  ```bash
  $ jupyter --version
  jupyter core     : 4.6.3
  jupyter-notebook : 6.0.3
  ...
  ```

  The traditional Jupyter notebook interface is more stable than Jupyter Lab and is recommended for this workshop.


## Test your setup

Please switch into the repository you downloaded in the previous step,
and run `python check_setup.py` to validate your installation.

On my computer, I see (but your version numbers may differ):

```
[✓] scikit-image  0.18.dev0
[✓] numpy         1.18.4
[✓] scipy         1.4.1
[✓] matplotlib    3.2.1
[✓] notebook      6.0.3
[✓] scikit-learn  0.23.0rc1
[✓] pandas        1.0.3
[✓] napari        0.3.6
```

**If you do not have a working setup, please contact the instructors.**

## After the workshop

We will upload our completed notebooks to the
`monash-df-2020-08-completed` branch. You can download it with git using:

```
git commit -a -m "Work completed in class"
git fetch origin monash-df-2020-08-completed
git switch monash-df-2020-08-completed
```

Or you can download them directly at:

https://github.com/jni/skimage-tutorials/archive/monash-df-2020-08-completed.zip


