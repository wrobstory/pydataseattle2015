# PyData Seattle 2015: Python Data Bikeshed

![3508571577_1a633e7bc4_z](https://cloud.githubusercontent.com/assets/2601457/8842529/354483d6-30b0-11e5-923c-0c72ea8e3b4d.jpg)

This repo contains the slides, data, and Jupyter Notebook for the PyData Seattle 2015 talk *Python Data Bikeshed*. The goal of the talk is to help answer the following question: 

> I have data.
> It’s July 2015.
> I want to group things.
> or count things.
> or average things.
> or add things.
> 
> **What Python library do I use?**

This talk discusses the following libraries in some depth: 

* Toolz: https://github.com/pytoolz/toolz
* Pandas: https://github.com/pydata/pandas
* Blaze: https://github.com/ContinuumIO/blaze
* xray: https://github.com/xray/xray
* bcolz: https://github.com/Blosc/bcolz
* Dask: https://github.com/ContinuumIO/dask

The following libraries or projects are briefly mentioned: 

* Cython: https://github.com/cython/cython
* Numexpr: https://github.com/pydata/numexpr
* Numba: https://github.com/numba/numba
* Numpy: https://github.com/numpy/numpy
* Spark: http://spark.apache.org/
* Bolt: http://bolt-project.org/
* Dato SArray: https://dato.com/products/create/docs/generated/graphlab.SArray.html
* Dato SFrame: https://dato.com/products/create/docs/generated/graphlab.SFrame.html#graphlab.SFrame
* DistArray: https://github.com/enthought/distarray
* Biggus: https://github.com/SciTools/biggus
* Spartan: https://github.com/spartan-array/spartan
* Ibis: https://github.com/cloudera/ibis
* scikit-learn: https://github.com/scikit-learn/scikit-learn
* statsmodels: https://github.com/statsmodels/statsmodels/
* Bokeh: https://github.com/bokeh/bokeh
* seaborn: https://github.com/mwaskom/seaborn

There is an example Notebook that goes into much more depth on the core libraries discussed in the talk; it can be read directly in Github, or on [nbviewer](http://nbviewer.ipython.org/github/wrobstory/pydataseattle2015/blob/master/PyDataSeattle2015.ipynb). 

If you would like to run the example yourself, you will need to either pip or conda install the follow dependencies: 
```
Babel==1.3
Cython==0.22.1
Jinja2==2.7.3
MarkupSafe==0.23
Pygments==2.0.2
SQLAlchemy==1.0.7
Sphinx==1.3.1
alabaster==0.7.6
backports.ssl-match-hostname==3.4.0.2
bcolz==0.10.0
blaze==0.8.2
certifi==2015.04.28
dask==0.6.0
datashape==0.4.6
decorator==3.4.2
dill==0.2.3
docutils==0.12
functools32==3.2.3-2
gnureadline==6.3.3
ipython==3.2.1
jsonschema==2.5.1
mistune==0.7
multipledispatch==0.4.8
networkx==1.9.1
nose==1.3.7
numexpr==2.4.3
numpy==1.9.2
numpydoc==0.5
odo==0.3.3
pandas==0.16.2
psutil==3.1.1
psycopg2==2.6.1
ptyprocess==0.5
python-dateutil==2.4.2
pytz==2015.4
pyzmq==14.7.0
requests==2.7.0
six==1.9.0
snowballstemmer==1.2.0
sphinx-rtd-theme==0.1.8
terminado==0.5
toolz==0.7.2
tornado==4.2.1
wsgiref==0.1.2
xray==0.5.2
```

The Blaze demo also requires installing Postgres, creating a `pydata` database, and populating a `diamonds` table with the correct schema. Postgres can be reliably installed with homebrew or conda, and the table created with the following SQL:
```
CREATE TABLE diamonds (
    carat     float,
    cut       varchar(255),
    color     varchar(255),
    clarity   varchar(255),
    depth     float, 
    "table"   float,  
    price     integer,
    x         float, 
    y         float, 
    z         float  
);
```
