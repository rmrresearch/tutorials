Setting Up a Research Project
=============================

Each project should be self contained. This includes not only the inputs, data,
and data analysis, but also the tools used to process and analyze the data. To
that end, Python's virtual environments are incredibly useful. With a Python
virtual environment all of your Python packages are saved as part of the project
and users only need to source the environment to get the same packages.

To make a virtual environment run:

.. code-block:: python

    python3 -m venv <name_of_env>

This will initialize an environment, but won't activate it. To activate it you
need to run:

.. code-block:: bash

    source <name_of_env>/bin/activate

This should change your command prompt to let you know that it worked. With your
environment loaded, the next step is to add the python packages you want. This
can be done using normal ``pip`` commands. For example, to add Jupyter notebooks
run:

.. code-block:: bash

    pip install jupyter

If you use jupyter notebooks you'll also probably want the ``nbextensions``
package, which can be retrieved and added to Jupyter by:

.. code-block:: bash
 
    pip install jupyter_contrib_nbextensions
    jupyter contrib nbextension install --sys-prefix


