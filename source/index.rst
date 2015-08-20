
lhcb-manual
===========

.. py:class:: DecayTreeTuple

Allows you to save event data in the `NTuple` (ROOT `TTree`) format.

The data is saved using individual :py:class:`TupleTool`\s, which have to be configured separately.
These are plugged into :py:class:`DecayTreeTuple` using the :py:attr:`ToolList` attribute.

When executing, the :py:class:`DecayTreeTuple` runs all of its :py:class:`TupleTool`\s, each of which saves entries to certain branches.

   .. py:function:: __init__(name)

      :param str name: The name to use for this instance of the DecayTreeTuple Algorithm.
                       This also defines the name of the tree inside the ROOT file.

   .. py:attribute:: ToolList
   
   A :py:class:`list` of :py:class:`str` with names of :py:class:`TupleTool`\s.
   Each of these will later be executed by the :py:class:`DecayTreeTuple`
   
   .. py:attribute:: TupleName

   The name of the directory that the DecayTreeTuple will save data to in your ROOT file.

.. toctree::
   :maxdepth: 2

Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`

