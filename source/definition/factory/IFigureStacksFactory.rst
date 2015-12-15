.. java:import:: java.util List

IFigureStacksFactory
====================

.. java:package:: Definition.factory
   :noindex:

.. java:type:: public interface IFigureStacksFactory

   Figure stack factory

Methods
-------
createFigureStack
^^^^^^^^^^^^^^^^^

.. java:method::  List<IFigureStack> createFigureStack(IBoard board, IBoardElement boardElement, Object payload)
   :outertype: IFigureStacksFactory

   The factory for creating figure stacks

   :param board: The board on which the stack is created
   :param boardElement: The board element on which the stack is created
   :param payload: A custom object that helps in creating the factory
   :return: The new figure stack

