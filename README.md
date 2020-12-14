## Machines Learn to Infer Stellar Parameters Just by Looking at a Large Number of Spectra
Here you can find the code and (pointers to) the data used in the paper: [arxiv.org/abs/2009.12872](https://arxiv.org/abs/2009.12872) ([DOI:10.1093/mnras/staa3540](https://dx.doi.org%2F10.1093%2Fmnras%2Fstaa3540&v=e626d26c))

![alt](http://www.eso.org/~nsedagha/universe/teaser.png "Machines")

<!--
If you use this code for research please cite:
   
    @InProceedings{sedaghat_machines_2020,
      author       = "N. Sedaghat and M. Zolfaghari and E. Amiri and T. Brox",
      title        = "Orientation-boosted voxel nets for 3D object recognition",
      booktitle    = "British Machine Vision Conference (BMVC)",
      month        = " ",
      year         = "2017",
      url          = "http://lmb.informatik.uni-freiburg.de/Publications/2017/SZB17a"
    }
-->

Please refer to the [main project page](http://www.eso.org/~nsedagha/universe) under the ESO website, to try out the 'sliders' and 'RETR-SPECT' interfaces.


## How to use
* Clone the repository to a local directory of your choice. e.g. ```machines```.
    * ```git clone git@github.com:NimSed/machines.git```
    * ```cd machines```

* Fetch the lists, metadata and labels for HARPS spectra:
    * ```cd lists```
    * ```sh fetch_lists.sh``` 
    * ```cd ..```

* Fetch the _encoded_ HARPS dataset:
    * ```cd encoded```
    * ```sh fetch_codes.sh``` 
    * ```cd ..```
    
* Play with the provided notebook to visualize the learned features and finally reproduce the plots in section 6 of the paper.
    * ```cd notebooks```
    * ```jupyter-notebook```
    
## Dependencies
```bash
pip3 install astropy
```
``` 
