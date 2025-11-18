# NGC Dataset creating you own DSO Target list 

I was curius to see what DSO (Deep Sky Objects) I may be omitting - and so I thought it would be interesting and insightful for a data exploration in the NGC Catalog.

The NGC catalog has been around for some time, but has often been somewhat messy to work with. 

I am please to say there is an excellent Python package called **pyongc**, which will make your life must easier.

## Installing pyongc 

**Assuming** python3.x, I would stringly suggest setting a virtual environment also (out of scope here) 

    pip install pyongc jupyter-lab pandas 

That is it. I believe you can use it on the command line - but I have not tried. 

## DataSet Creation 

Please look at the supplied Jupyter Notebook  file [NGCFiltering.ipynb](./NGCFiltering.ipynb)

The output of this file is a *feather* file (a data storage), which can be processed in another step.

I used the *mean* **size** and **brightness** of the *Messier* catalog, and then filtered the NGC catalog for items which are

  - brighter than the messier mean
  - bigger and brighter than the messier mean
  - bigger than the messier mean 

Finally I picked all items which have a commonname. 

The number of records per grouping is 

  - large_bright_df has 29 records
  - large_df has 85 records
  - bright_df has 176 records
  - common_named_objects has 122 records

I made sure there were no duplicates, and then saved them as a output datafile.

We have 412 potential objects now.
Instead of 110 messier objects.
There are in total 14033 ngc objects in total.


## Further refinement ?

If you only want OpenClusters, Nebular or Oi Galaxies  - this all can be filtered. Just play with the notebook. 
