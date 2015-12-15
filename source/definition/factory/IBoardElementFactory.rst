.. java:import:: Definition IBoard

.. java:import:: Definition IBoardElement

IBoardElementFactory
====================

.. java:package:: Definition.factory
   :noindex:

.. java:type:: public interface IBoardElementFactory

   Board element factory

Methods
-------
createBoardElement
^^^^^^^^^^^^^^^^^^

.. java:method::  IBoardElement createBoardElement(IBoard board, Object payload)
   :outertype: IBoardElementFactory

   The factory for creating board elements

   :param board: The board on which the element is created
   :param payload: A custom object that helps in creating the factory
   :return: The new board element

