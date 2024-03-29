almirah
=======

.. toctree::
   :hidden:

   user-guide
   tutorial
   writing-configs/index
   adbs/index
   reference/index
   contributing
   code-of-conduct   
   changelog

almirah aids in the organization, maintenance, and usage of both
file-based and table-based datasets. Developed to handle neuroimaging
datasets, it provides data format conversion support for specific
modalities.

Out-of-the-box, almirah supports:

- BIDS specification for neuroimaging datasets.
- BIDS-like specification for genome sequence data.
- Interfacing with databases supported by SQLAlchemy.
- File format conversion for neuorimaging data.
- Lazy access of DataLad compatible datasets.

With some time on config writing, almirah can:

- Organize unformatted datasets.
- Query and filter across the dataset.
- Migrate records from one database to another.

Installing
----------

almirah can be installed with `pip <https://pip.pypa.io>`_:

.. code-block:: bash
		
		$ python -m pip install almirah

Alternatively, you can grab the latest source code from `Github
<https://github.com/girishmm/almirah>`_:

.. code-block:: bash

		$ git clone https://github.com/girishmm/almirah.git
		$ cd almirah
		$ pip install .

Usage
-----

The :doc:`user-guide` is the place to go to learn how to use the
libray and accomplish common dataset related tasks. If you have the
time, we recommend following the :doc:`tutorial` for a complete
overview.

almirah relies heavily on configs to guide its tasks. The
:doc:`writing-configs/index` page describes the possibilities in
detail.

If you want to access the ADBS dataset, please head over to
:doc:`adbs/tutorial` for a walk-through. The
:doc:`adbs/reference/index` documentation provides details on the
files and records available in the dataset. If you have not heard of
the ADBS study, but would like to know, :doc:`adbs/index` page can
help acquaint you.

The :doc:`reference/index` documentation provides API-level
documentation.

Can you use almirah to manage your dataset? Of course. Have a look at
:ref:`translate` section for files to tweak to achieve this.

Who uses almirah?
--------------

almirah was primarily developed to support and maintain the data
generated by the ADBS study. But we believe it can aid with other
datasets too! Even non-neuroimaging ones!

If almirah was able to help with your dataset, we would love to hear
about it.

.. _translate:

Translate to another dataset
----------------------------

If your dataset is a BIDS dataset, congrats you are done! 🎉

If you dataset follows a different specification, describe it as a
config file by referring to :doc:`writing-configs/specification`. This
should allow filtering and querying of the dataset.

If you would like to organize data according to a described
specification, define rules according to :doc:`writing-configs/rules`.

If you need assistance migrating records from one database to another,
or one schema to another, :doc:`writing-configs/mapping` can guide
you.

License
-------

almirah is made available under the MIT License. For more details, see
`LICENSE <https://github.com/girishmm/almirah/blob/dev/LICENSE>`_.

Contributing
------------

We happily welcome contributions, please see :doc:`contributing` for
details.

Help and Support
----------------

We try to make almirah robust, but there might be things we missed. If it
does not meet your use case or you have trouble adapting it to your
dataset, please `write to us <girishmm@ncbs.res.in>`_ or open an issue
on the `repository <https://github.com/girishmm/almirah>`_ or drop by
`Github Discussions <https://github.com/girishmm/almirah/discussions>`_.

Citing
------

If you use almirah to help with your dataset, please consider citing this
repository until a journal article is specifically available for almirah.

If you use the ADBS dataset in your research, please cite the
reference below until a journal article is available for the dataset:

.. code-block:: text
		
    Viswanath, B., Rao, N.P., Narayanaswamy, J.C. et al. Discovery
    biology of neuropsychiatric syndromes (DBNS): a center for
    integrating clinical medicine and basic science. BMC Psychiatry
    18, 106 (2018). doi: https://doi.org/10.1186/s12888-018-1674-2.

Acknowledgements
----------------

almirah builds on other libraries and some parts are implemented as a
wrapper around modules in these libraries. Thanks to the developers,
maintainers, and contributors of these for the amazing documentation
and great work!

- mne
- mne-bids
- mne-nirs
- dcm2bids
- pybids  
- SQLAlchemy

.. rubric:: References

- Alexandre Gramfort, Martin Luessi, Eric Larson, Denis A. Engemann,
  Daniel Strohmeier, Christian Brodbeck, Roman Goj, Mainak Jas, Teon
  Brooks, Lauri Parkkonen, and Matti S. Hämäläinen. MEG and EEG data
  analysis with MNE-Python. Frontiers in Neuroscience,
  7(267):1–13, 2013. doi: https://doi.org/10.3389/fnins.2013.00267.
  
- Appelhoff, S., Sanderson, M., Brooks, T., Vliet, M., Quentin, R.,
  Holdgraf, C., Chaumon, M., Mikulan, E., Tavabi, K., Höchenberger,
  R., Welke, D., Brunner, C., Rockhill, A., Larson, E., Gramfort, A.,
  & Jas, M. (2019). MNE-BIDS: Organizing electrophysiological data
  into the BIDS format and facilitating their analysis. Journal of
  Open Source Software, 4:1896. doi:
  https://doi.org/10.21105/joss.01896.
  
- Robert Luke, Eric D. Larson, Maureen J. Shader, Hamish Innes-Brown,
  Lindsey Van Yper, Adrian K. C. Lee, Paul F. Sowman, David
  McAlpine. Analysis methods for measuring passive auditory fNIRS
  responses generated by a block-design paradigm. Neurophotonics,
  Vol. 8, Issue 2, 025008 (May 2021). doi:
  https://doi.org/10.1117/1.NPh.8.2.025008.
  
- Boré, A., Guay, S., Bedetti, C., Meisler, S., &
  GuenTher, N. (2023). Dcm2Bids (Version 3.0.2) [Computer
  software]. doi: https://doi.org/10.5281/zenodo.8306314.
  
- Yarkoni et al., (2019). PyBIDS: Python tools for BIDS
  datasets. Journal of Open Source Software, 4(40), 1294.  doi:
  https://doi.org/10.21105/joss.01294.





