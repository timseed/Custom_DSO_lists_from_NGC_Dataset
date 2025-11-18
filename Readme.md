# NGC Dataset creating you own DSO Target list 

I was curius to see what DSO (Deep Sky Objects) I may be omitting - and so I thought it would be interesting and insightful for a data exploration in the NGC Catalog.

The NGC catalog has been around for some time, but has often been somewhat messy to work with. 

I am please to say there is an excellent Python package called **pyongc**, which will make your life must easier.

## Installing pyongc 

**Assuming** python3.x, I would stringly suggest setting a virtual environment also (out of scope here) 

    pip insall pyongc 

That is it. I believe you can use it on the command line - but I have not tried. 

## DataSet Creation 

Please look at the supplied Jupyter Notebook  file [NGCFiltering.ipynb](./NGCFiltering.ipynb)

The output of this file is a *feather* file (a data storage), which can be processed in another step.
