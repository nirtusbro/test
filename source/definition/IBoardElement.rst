IBoardElement
=============

.. java:package:: Definition
   :noindex:

.. java:type:: public interface IBoardElement extends IMetadataCore, IRenderable

   One board element, is renderable and contains several figure stacks

Methods
-------
addFigureStack
^^^^^^^^^^^^^^

.. java:method::  IFigureStack addFigureStack(IFigureStack stack)
   :outertype: IBoardElement

addFigureStack
^^^^^^^^^^^^^^

.. java:method::  IFigureStack addFigureStack(IFigureStack stack, String name)
   :outertype: IBoardElement

   Adds a figure stack

   :param stack: Figure stack to be added
   :param name: Stack name
   :return: The added stack

addFigureStacks
^^^^^^^^^^^^^^^

.. java:method::  List<IFigureStack> addFigureStacks(List<IFigureStack> stacks)
   :outertype: IBoardElement

connectTo
^^^^^^^^^

.. java:method::  IBoardElement connectTo(IBoardElement target, int cost)
   :outertype: IBoardElement

   Connects this element with another

   :param target: Target element
   :param cost: Cost in that direction
   :return: The target element

getAllConnectedBoardElements
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method::  Map<IBoardElement, Integer> getAllConnectedBoardElements()
   :outertype: IBoardElement

   Returns all the board elements that are connected

   :return: A map of connected elements

getAllUnvisitedConnectedElements
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method::  Map<IBoardElement, Integer> getAllUnvisitedConnectedElements()
   :outertype: IBoardElement

   Returns all the board elements that are connected and where !isVisited()

   :return: A map of unvisited connected elements

getDefaultFigure
^^^^^^^^^^^^^^^^

.. java:method::  IFigure getDefaultFigure()
   :outertype: IBoardElement

   Returns the default figure for this element, null if it is nonexistent or the element doesn't have any stacks. The default figure is the figure that was first created on the stack that was first created.
	
   :return: The default figure

getDefaultStack
^^^^^^^^^^^^^^^

.. java:method::  IFigureStack getDefaultStack()
   :outertype: IBoardElement

   Returns the default stack, null if it is nonexistent. The default stack is the stack that was first created.

   :return: The default stack

getFigureStacks
^^^^^^^^^^^^^^^

.. java:method::  List<IFigureStack> getFigureStacks()
   :outertype: IBoardElement

   Returns the figure stacks

   :return: Figure stacks

getFigureStacks
^^^^^^^^^^^^^^^

.. java:method::  IFigureStack getFigureStacks(String name)
   :outertype: IBoardElement

   Returns a stack figure with the given name

   :param name: Figure name
   :return: Figure stack

getUniqueName
^^^^^^^^^^^^^

.. java:method::  String getUniqueName()
   :outertype: IBoardElement

   Returns the unique name

   :return: Board element name

isVisited
^^^^^^^^^

.. java:method::  boolean isVisited()
   :outertype: IBoardElement

   Returns a boolean value which represents whether or not the element is visited

   :return: true if it is, false if it isn't

setUniqueName
^^^^^^^^^^^^^

.. java:method::  void setUniqueName(String name)
   :outertype: IBoardElement

   Sets the unique name

   :param name: Unique name to be set

setVisited
^^^^^^^^^^

.. java:method::  void setVisited(boolean visited)
   :outertype: IBoardElement

   Sets the element to visited, i.e. sets the boolean visited to true

   :param visited: true if it is, false if it isn't

