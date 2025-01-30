## Astro-Machines:
## Machines Learn to Infer Stellar Parameters Just by Looking at a Large Number of Spectra
Here you can find the code and (pointers to) the data used in the paper: [arxiv.org/abs/2009.12872](https://arxiv.org/abs/2009.12872) ([DOI:10.1093/mnras/staa3540](https://dx.doi.org/10.1093/mnras/staa3540))

![alt](https://www.rawdataspeaks.org/wp-content/uploads/2022/05/autoencoder-teaser_new.png "Astro-Machines")

<!--
If you use this code for research please cite:
   @article{sedaghat2021machines,
     title={Machines learn to infer stellar parameters just by looking at a large number of spectra},
     author={Sedaghat, Nima and Romaniello, Martino and Carrick, Jonathan E and Pineau, Fran{\c{c}}ois-Xavier},
     journal={Monthly Notices of the Royal Astronomical Society},
     volume={501},
     number={4},
     pages={6026--6041},
     year={2021},
     publisher={Oxford University Press}
   }

-->

Please refer to the [main project page](https://www.rawdataspeaks.org/projects/astro-machines), to try out the 'sliders' and 'RETR-SPECT' interfaces.


## How to use
* Clone the repository to a local directory of your choice. e.g. ```astro-machines```.
    * ```git clone https://github.com/NimSed/astro-machines.git```
    * ```cd astro-machines```

* Extract the lists, metadata and labels for HARPS spectra:
    * ```cd lists```
    * ```tar xfz list.tar.gz``` 
    * ```cd ..```
    
* Play with the provided notebook to visualize the learned features and finally reproduce the plots in section 6 of the paper.
    * ```cd notebooks```
    * ```jupyter-notebook```

### Optional -- to pass individual HARPS-like spectra through pretrained networks
* Fetch pretrained models:
    * ```cd models```
    * ```sh fetch_models.sh``` 
    * ```cd ..```

* Test/infer on the provided sample.fits:
    * ```cd infer```
    * ```python3 infer.py```

You can of course use an arbitrarily chosen HARPS spectrum (in fits format). Just pass it to infer.py using the ```--fits_file``` argument.

## Dependencies
```bash
pip3 install astropy
```

