# post_processing_tests

Examples of PSF photon counting and PSF subtraction using open source post-processing libraries [pyKLIP](https://bitbucket.org/pyKLIP/pyklip) [PynPoint](https://github.com/PynPoint/PynPoint).

Photon counting follows the recipe described in [Ygouf et al 2020](https://roman.ipac.caltech.edu/docs/sims/20210110_Roman_CGI_post_processing_report_URS_corrected_typo.pdf)

[Roman_Ygouf_Pyklip_HDF5.ipynb](Roman_Ygouf_Pyklip_HDF5.ipynb):
-imports Roman OS9 test data (prior notebook, same name)
-runs it through first or third order photon counting (prior notebook, same name)
-runs a deepcopy of photon counted OS9 data through Pyklip RDI and ADI
-converts photon counted OS9 data into HDF5 for processing by Pynpoint

[Roman_OS9_Pynpoint.ipynb](Roman_OS9_Pynpoint.ipynb)
-imports the HDF5 file that was prepared by Roman_Ygouf_Pyklip_HDF5.ipynb
-runs that photon counted OS9 data through RDI and ADI, using 
