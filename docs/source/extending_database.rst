------------------
Extending database
------------------

Since, the thermochemical database is fed via dictionary (``dict_of_all_sp_grt``), the thermochemical database can be easily modified by either providing NASA 9 polynomial in ``thermo_dict`` or directly providing chemical potentials to ``dict_of_all_sp_grt`` at specified temperature.


.. code-block::
    :linenos:

    thermo_dict, stoichiometric_dict = pythermoread.thermoread()
    dict_of_all_sp_grt = pythermoread.calculate_grt(grt_dict, temperature, thermo_dict)

----------
References
----------
.. [Kenneth1956] Kenneth Denbigh, 1956. The Principles of Chemical Equilibrium, with Applications in Chemistry and Chemical Engineering., :math:`4^{th}` Edition. Cambridge University Press, Cambridge.