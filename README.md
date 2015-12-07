# Blowing the doors off your bottlenecks with Python on AMD APUs
## Stan Seibert<br/>December 8, 2015

(This notebook contains code from a webinar showing how to use Python and Numba to write code that takes advantage of the GPU-capabilities on AMD APUs.  For a recording of this webinar, see: TBD)

This example requires:
 * An AMD APU: Kaveri and Carrizo processors have been tested
 * Ubuntu Linux 14.04 64-bit
 * [AMD HSA 1.0 final drivers](https://github.com/HSAFoundation/HSA-Docs-AMD/wiki/HSA-Platforms-&-Installation)

The easiest way to test out the code in this notebook is to download [Miniconda](http://conda.pydata.org/miniconda.html) and run the following commands to create and activate a new environment:
```
conda create -n hsa_webinar python=3.4 numba libhlc pandas bokeh matplotlib basemap jupyter
source activate hsa_webinar
export LD_LIBRARY_PATH=/opt/hsa/lib

jupyter notebook
```
