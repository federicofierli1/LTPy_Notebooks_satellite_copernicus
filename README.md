# LTPy - Learning tool for Python on Atmospheric Composition Data

**LTPy - Learning tool for Python on Atmospheric Composition Data** is a 
Python-based training course on Atmospheric Composition Data. The training 
course covers modules on data access, data handling and processing, 
data visualisation as well as case studies of satellite- and model-based data 
on Atmospheric Composition.

The course is based on [Jupyter notebooks](https://jupyter.org/), which allow 
for a high-level of interactive learning, as code, text description and 
visualisation is combined in one place.

## Data on Atmospheric Composition
This course features the following data:

This course features the following data:
* [AC SAF Level-2 GOME-2](./1_ltpy_v01_atmospheric_composition_overview.ipynb#ac_saf) 
data onboard of Metop-A and Metop-B satellites
* [AC SAF Level-3 GOME-2](./1_ltpy_v01_atmospheric_composition_overview.ipynb#records) 
reprocessed and regridded data
* [Copernicus Sentinel-5P](./1_ltpy_v01_atmospheric_composition_overview.ipynb#sentinel_5p) 
data

# Course structure
The course follows a modular approach and offers the following modules:

* **1 - Overview of data and data access systems**
 * [1 - Atmospheric Composition data overview and acccess](./1_ltpy_v01_atmospheric_composition_overview.ipynb)
* **2 - Load and browse data**
 * [2.1 - AC SAF Level 2 data](./21_ltpy_v01_AC_SAF_L2_data.ipynb)
 * [2.2 - AC SAF Level 3 data](./22_ltpy_v01_AC_SAF_L3_data_products.ipynb)
 * [2.3 - Sentinel-5p Level 2 data](./23_ltpy_v01_Sentinel5p_L2_data.ipynb)
* **3 - Data workflows and case studies**
 * [3.1 - AC SAF Level 2 case studies](./31_ltpy_v01_AC_SAF_L2_case_study.ipynb)
 * [3.2 - AC SAF Level 3 workflow examples](./32_ltpy_v01_AC_SAF_L3_case_study.ipynb)

Optional: the module "[**Introduction to Python and Project Jupyter**](./0_ltpy_v01_Intro_to_Python_and_Jupyter,ipynb)" 
gives you a head start to the Python and Jupyter knowledge you might find 
helpful in order to follow this course.

# Learning outcomes
The course is designed for `medium-level users`, who have basic Python knowledge 
and understanding of `Atmospheric composition data`.

After the course, you should have:

* an idea about the different datasets on Atmospheric Composition data,
* knowledge about the most useful Python packages to handle, process and 
visualise large volumes of Earth Observation data
* an idea about different data application areas

# How to use this course material
This course material is made available via EUMETSAT's eo-lab training space on
GitLab. While GitLab offers integrated rendering of Jupyter Notebooks, it's 
rendering capabilities is limited. Thus, the notebooks, if directly rendered on
GitLab, might appear not in a nice format, which make the learning process
difficult.

There are several ways how to use these modules:
* 1. **[nbviewer](https://nbviewer.jupyter.org/)** - Static rendering of the 
notebooks. Copy paste the link to the notebook [index_ltpy_v01.ipynb](./index_ltpy_v01.ipynb) 
into nbviewer.
* 2. **Clone this repo** and run the notebooks on your local Jupyter notebook
server. If you prefer this solution, you have to reproduce the settings. Under 
the "Technical requirements" section, you find more information on how to
reproduce the set up on your local machine.
* 3. **LTPy JupyterHub** - You can create a 
[WEkEO account](https://www.wekeo.eu/user/register) and then log into the
[LTPy Jupyterhub](https://ltpy.adamplatform.eu).

# Technical requirements
The notebooks have been developed under `Python3`. 

The following `Python packages` will be needed in order to reproduce the 
LTPy examples on your local setup:
* [xarray](http://xarray.pydata.org/en/stable/index.html)
* [netCDF4](https://unidata.github.io/netcdf4-python/netCDF4/index.html)
* [h5py](https://pypi.org/project/h5py/)
* [numpy](https://numpy.org/)
* [matplotlib](https://matplotlib.org/)
* [cartopy](https://scitools.org.uk/cartopy/docs/latest/)

The following `data` are required to be downloaded:
| Satellite | Data type | Parameter | Temporal coverage | Data Volume
|--- |---|---|---|---|
|GOME-2 - Metop-2a|Level-2 Offline| `Nitrogen Dioxide`  |`18-Aug-2019` <br> `19-Aug-2019` <br> `22-Aug-2019`| 222 MB <br> 214 MB <br> 212 MB |
|GOME-2 - Metop-2b|Level-2 Offline| `Nitrogen Dioxide`  |`18-Aug-2019` <br> `19-Aug-2019` <br> `22-Aug-2019`| 221 MB <br> 219 MB <br> 232 MB |
|GOME-2 - Metop-2a|Level-2 Offline| `Nitrogen Dioxide`  |`13-Aug-2018` <br> `16-Aug-2018` <br> `18-Aug-2018`| 222 MB <br> 214 MB <br> 212 MB |
|GOME-2 - Metop-2b|Level-2 Offline| `Nitrogen Dioxide`  |`13-Aug-2018` <br> `16-Aug-2018` <br> `18-Aug-2018`| 222 MB <br> 214 MB <br> 212 MB |
|GOME-2 - Metop-2a|Level-3 Data record| `Nitrogen Dioxide`  |`Feb-2007 - Dec-2012`| 4.78 GB |
|GOME-2 - Metop-2b|Level-3 Data record| `Nitrogen Dioxide`  |`Jan-2013 - Nov-2017`| 4 GB |
|GOME-2 - Metop-2b|Level-3 Data record| `Tropical tropospheric Ozone`  |`Jan-Dec 2018`| 5.1 MB |
|Sentinel-5P TROPOMI|Level-2 Offline| `Nitrogen Dioxide`  |`13-Aug-2018` <br> `16-Aug-2018` <br> `18-Aug-2018`| 1.35 GB <br> 1.37 GB <br> " " |
|Sentinel-5P TROPOMI|Level-2 Offline| `Nitrogen Dioxide`  |`19-Aug-2019` <br> `22-Aug-2019`| 1.82 GB <br> 1.37 GB |
