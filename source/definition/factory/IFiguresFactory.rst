.. java:import:: Definition IBoard

.. java:import:: Definition IBoardElement

.. java:import:: Definition IFigureStack

.. java:import:: java.util List

IFiguresFactory
===============

.. java:package:: Definition.factory
   :noindex:

.. java:type:: public interface IFiguresFactory

   Created by hades-incarnate on 11/2/2015. Fabrika elemenata

Methods
-------
createFigures
^^^^^^^^^^^^^

.. java:method::  List<IFigureStack> createFigures(IBoard board, IBoardElement boardElement, IFigureStack stack, Object payload)
   :outertype: IFiguresFactory

   Fabrika za kreiranje figura

   :param board: board na kome se kreira figura
   :param boardElement: board element na kome se kreira figura
   :param stack: stack na kome se kreira figura
   :param payload: custom objekat koji pomaze u kreiranju
   :return: Novi figure stack

