.. java:import:: Definition IMetadataCore

.. java:import:: java.util HashMap

.. java:import:: java.util Map

MetadataContainer
=================

.. java:package:: Source
   :noindex:

.. java:type:: public abstract class MetadataContainer implements IMetadataCore

   Created by hades-incarnate on 10/30/2015. implementacija storage-a za metadata

Constructors
------------
MetadataContainer
^^^^^^^^^^^^^^^^^

.. java:constructor:: public MetadataContainer()
   :outertype: MetadataContainer

Methods
-------
createMetadataValue
^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void createMetadataValue(String key, Object value)
   :outertype: MetadataContainer

   Pravi hash mapu

   :param key: Kljuc
   :param value: Vrednost

getAllMetadataValues
^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public Map<String, Object> getAllMetadataValues()
   :outertype: MetadataContainer

   Vraca sve kljuceve i vrednosti

   :return: Kljucevi i vrednosti

getMetadataValue
^^^^^^^^^^^^^^^^

.. java:method:: @Override public Object getMetadataValue(String key)
   :outertype: MetadataContainer

   Vraca vrednost na osnovu kljuca

   :param key: Kljuc
   :return: Vrednost

updateMetadataValues
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void updateMetadataValues(Map<String, Object> values)
   :outertype: MetadataContainer

   Azuriranje vrednosti

   :param values: Vrednost koja se azurira

