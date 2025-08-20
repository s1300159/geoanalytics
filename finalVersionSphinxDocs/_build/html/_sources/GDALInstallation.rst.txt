Installation using Anaconda (geoanalytics package).
==================================================

`GDAL` is an important toolkit in our library. It is for converting the raster data in any format into a human readable text or CSV format.
We have present the methods to install this toolkit using Conda environment on a machine running Ubuntu operating system.

.. _installation-pip:

.. code-block:: console

   (.venv) $ sudo apt-get update && sudo apt upgrade -y && sudo apt autoremove

   (.venv) $ sudo apt-get install -y cdo nco gdal-bin libgdal-dev

   (.venv) $ pip install --global-option=build_ext --global-option="-I/usr/include/gdal" GDAL==`gdal-config --version`

   (.venv) $ python -m pip install --upgrade pip setuptools wheel

   (.venv) $ python -m pip install --upgrade gdal

**If the above two commands have failed to install gdal, then execute the following commands:**

.. code-block:: console

   (.venv) $ conda install -c conda-forge libgdal

   (.venv) $ conda install -c conda-forge gdal

   (.venv) $ conda install tiledb=2.2

   (.venv) $ conda install poppler

**Once the above commands were executed, check the version information by typing the following command on the `terminal`:**

.. code-block:: console

   (.venv) $ ogrinfo --version




