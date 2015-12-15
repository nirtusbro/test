.. java:import:: java.util Map

IMetadataCore
=============

.. java:package:: Definition
   :noindex:

.. java:type:: public interface IMetadataCore

   A metadata sysyem for custom game information

Methods
-------
createMetadataValue
^^^^^^^^^^^^^^^^^^^

.. java:method::  void createMetadataValue(String key, Object value)
   :outertype: IMetadataCore

   Makes a hash map of keys and their values

   :param key: The key
   :param value: The value

getAllMetadataValues
^^^^^^^^^^^^^^^^^^^^

.. java:method::  Map<String, Object> getAllMetadataValues()
   :outertype: IMetadataCore

   Returns a map of keys and their values

   :return: A map of keys and their values

getMetadataValue
^^^^^^^^^^^^^^^^

.. java:method::  Object getMetadataValue(String key)
   :outertype: IMetadataCore

   Returns a value based on the specified key

   :param key: The key
   :return: The value

