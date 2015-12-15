.. java:import:: Definition IBoard

.. java:import:: Definition IBoardElement

.. java:import:: Definition IFigureStack

.. java:import:: java.util List

IFiguresFactory
===============

.. java:package:: Definition.factory
   :noindex:

.. java:type:: public interface IFiguresFactory

   Element factory

Methods
-------
createFigures
^^^^^^^^^^^^^

.. java:method::  List<IFigureStack> createFigures(IBoard board, IBoardElement boardElement, IFigureStack stack, Object payload)
   :outertype: IFiguresFactory

   The factory for creating figures

   :param board: The board on which the figure is created
   :param boardElement: The board element on which the figure is created
   :param stack: The figure stack on which the figure is created
   :param payload: A custom object that helps in creating the factory
   :return: The new figure stack

