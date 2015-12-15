.. java:import:: java.util List

IFigureStack
============

.. java:package:: Definition
   :noindex:

.. java:type:: public interface IFigureStack extends IMetadataCore, IRenderable

   One board element can have several stacks at different locations, the stack defines the domain and order of figures. The figures' rendering is determined by an internal order.

Methods
-------
addFigure
^^^^^^^^^

.. java:method::  IFigure addFigure(IFigure figure, String name)
   :outertype: IFigureStack

   Adds a figure the list of figures

   :param figure: Figure to be added
   :param name: Name of the figure to be added
   :return: The added figure

addFigures
^^^^^^^^^^

.. java:method::  List<IFigure> addFigures(List<IFigure> figures)
   :outertype: IFigureStack

   Adds a list of figures to the list of figure lists

   :param figures: List of figures to be added
   :return: Added figures

getDefaultFigure
^^^^^^^^^^^^^^^^

.. java:method::  IFigure getDefaultFigure()
   :outertype: IFigureStack

   Returns the default figure from the stack, null if it is nonexistent. The default figure is the figure that was first created on the stack.

   :return: The default figure

getFigure
^^^^^^^^^

.. java:method::  IFigure getFigure(String name)
   :outertype: IFigureStack

   Returns a figure specified by its name from the stack

   :param name: Name of the figure
   :return: The required figure

getFigures
^^^^^^^^^^

.. java:method::  List<IFigure> getFigures()
   :outertype: IFigureStack

   Returns the list of figures

   :return: The list of figures

getName
^^^^^^^

.. java:method::  String getName()
   :outertype: IFigureStack

   Returns the figure's name

   :return: Figure's name

hasFigures
^^^^^^^^^^

.. java:method::  boolean hasFigures()
   :outertype: IFigureStack

   Returns a boolean value which represents whether or not the stack has figures

   :return: True if it has, false if it doesn't

setName
^^^^^^^

.. java:method::  void setName(String name)
   :outertype: IFigureStack

   Sets the figure's name

   :param name: Figure's name

