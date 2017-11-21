ipyleaflet
==========

A Jupyter / Leaflet bridge enabling interactive maps in the Jupyter notebook.

![Screenshot](/screenshot.png)

Getting Started
---------------

### Try it online with [Binder](http://mybinder.org/)

[![Binder](http://mybinder.org/badge.svg)](http://mybinder.org:/repo/ellisonbg/ipyleaflet/notebooks/examples)

Your first map
-------------

```
import ipyleaflet
map = ipyleaflet.Map(center=[37.9714, 23.7265], zoom=17)
map
```

A map centered on the Pantheon in Greece, rendered inline in your Jupyter Notebook should have appeared.


Installation
------------

Using pip:

```
$ pip install ipyleaflet
$ jupyter nbextension enable --py --sys-prefix ipyleaflet
```

Using conda:

```
$ conda install -c conda-forge ipyleaflet
```

If you have JupyterLab, you will also need to install the JupyterLab extension:

```
$ jupyter labextension install jupyter-leaflet
```

For a development installation (requires npm):

```
$ git clone https://github.com/ellisonbg/ipyleaflet.git
$ cd ipyleaflet
$ pip install -e .
$ jupyter nbextension install --py --symlink --sys-prefix ipyleaflet
$ jupyter nbextension enable --py --sys-prefix ipyleaflet
```

Note for developers: the `--symlink` argument on Linux or OS X allows one to
modify the JavaScript code in-place. This feature is not available
with Windows.


