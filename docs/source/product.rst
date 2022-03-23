Product
=====


Project Timeline
------------

.. list-table:: Tentative Dates
   :widths: 60 30
   :header-rows: 1

   * - Action
     - Tentative Date
   * - Beta Deployment
     - April 2021
   * - Soft Launch
     - February 2022
   * - Optimised Release
     - May 2022

To use Lumache, first install it using pip:

.. code-block:: console

   (.venv) $ pip install lumache

Creating recipes
----------------

To retrieve a list of random ingredients,
you can use the ``lumache.get_random_ingredients()`` function:

.. autofunction:: lumache.get_random_ingredients

The ``kind`` parameter should be either ``"meat"``, ``"fish"``,
or ``"veggies"``. Otherwise, :py:func:`lumache.get_random_ingredients`
will raise an exception.

.. autoexception:: lumache.InvalidKindError

For example:

>>> import lumache
>>> lumache.get_random_ingredients()
['shells', 'gorgonzola', 'parsley']

