# post_processing_tests

[Roman_Ygouf_Pyklip_HDF5.ipynb](Roman_Ygouf_Pyklip_HDF5.ipynb):
-imports Roman OS9 test data (prior notebook, same name)
-runs it through first or third order photon counting as per Ygouf recipe (prior notebook, same name)
-runs a deepcopy of photon counted OS9 data through Pyklip RDI and ADI
-converts photon counted OS9 data into HDF5 for processing by Pynpoint

[Roman_OS9_Pynpoint.ipynb](Roman_OS9_Pynpoint.ipynb)
-imports the HDF5 file that was prepared by Roman_Ygouf_Pyklip_HDF5.ipynb
-runs that photon counted OS9 data through RDI and ADI, using https://github.com/PynPoint/PynPoint
