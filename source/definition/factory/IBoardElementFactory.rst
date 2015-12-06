.. java:import:: Definition IBoard

.. java:import:: Definition IBoardElement

IBoardElementFactory
====================

.. java:package:: Definition.factory
   :noindex:

.. java:type:: public interface IBoardElementFactory

   Created by hades-incarnate on 10/31/2015. Fabrika board elemenata

Methods
-------
createBoardElement
^^^^^^^^^^^^^^^^^^

.. java:method::  IBoardElement createBoardElement(IBoard board, Object payload)
   :outertype: IBoardElementFactory

   Fabrika za kreiranje board elemenata

   :param board: board na kome se kreira element
   :param payload: custom objekat koji pomaze u kreiranju
   :return: novi Board Element

