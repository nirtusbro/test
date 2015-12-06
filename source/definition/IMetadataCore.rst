.. java:import:: java.util Map

IMetadataCore
=============

.. java:package:: Definition
   :noindex:

.. java:type:: public interface IMetadataCore

   Created by hades-incarnate on 10/20/2015. metadata sistem za custom game podatke, napraviti od ovoga core klasu koja ce biti nasledjivana u svim klasama koje implementiraju interfejse nasledjene of ovog .

Methods
-------
createMetadataValue
^^^^^^^^^^^^^^^^^^^

.. java:method::  void createMetadataValue(String key, Object value)
   :outertype: IMetadataCore

   Pravi hash mapu

   :param key: Kljuc
   :param value: Vrednost

getAllMetadataValues
^^^^^^^^^^^^^^^^^^^^

.. java:method::  Map<String, Object> getAllMetadataValues()
   :outertype: IMetadataCore

   Vraca sve kljuceve i vrednosti

   :return: Kljucevi i vrednosti

getMetadataValue
^^^^^^^^^^^^^^^^

.. java:method::  Object getMetadataValue(String key)
   :outertype: IMetadataCore

   Vraca vrednost na osnovu kljuca

   :param key: Kljuc
   :return: Vrednost

