.. java:import:: Definition IMetadataCore

.. java:import:: java.util HashMap

.. java:import:: java.util Map

MetadataContainer
=================

.. java:package:: Source
   :noindex:

.. java:type:: public abstract class MetadataContainer implements IMetadataCore

   The implementation of metadata storage

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

   Makes a hash map of keys and their values

   :param key: The key
   :param value: The value

getAllMetadataValues
^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public Map<String, Object> getAllMetadataValues()
   :outertype: MetadataContainer

   Returns a map of keys and their values

   :return: A map of keys and their values

getMetadataValue
^^^^^^^^^^^^^^^^

.. java:method:: @Override public Object getMetadataValue(String key)
   :outertype: MetadataContainer

   Returns a value based on the specified key

   :param key: The key
   :return: The value

updateMetadataValues
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void updateMetadataValues(Map<String, Object> values)
   :outertype: MetadataContainer

   Updates metadata values

   :param values: Values to be updated

