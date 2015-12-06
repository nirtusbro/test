.. java:import:: java.util List

IFigureStacksFactory
====================

.. java:package:: Definition.factory
   :noindex:

.. java:type:: public interface IFigureStacksFactory

   Created by hades-incarnate on 11/2/2015. Fabrika stackova elemenata

Methods
-------
createFigureStack
^^^^^^^^^^^^^^^^^

.. java:method::  List<IFigureStack> createFigureStack(IBoard board, IBoardElement boardElement, Object payload)
   :outertype: IFigureStacksFactory

   Fabrika za kreiranje stackova elemenata

   :param board: board na kome se kreira stack
   :param boardElement: board element na kome se kreira stack
   :param payload: custom objekat koji pomaze u kreiranju
   :return: Novi figure stack

