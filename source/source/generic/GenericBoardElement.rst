.. java:import:: Source RenderableMetadataContainer

.. java:import:: java.util List

.. java:import:: java.util.stream Collectors

GenericBoardElement
===================

.. java:package:: Source.generic
   :noindex:

.. java:type:: public class GenericBoardElement extends RenderableMetadataContainer implements IBoardElement

   Generic board element

Constructors
------------
GenericBoardElement
^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public GenericBoardElement(IBoard board)
   :outertype: GenericBoardElement

Methods
-------
addFigureStack
^^^^^^^^^^^^^^

.. java:method:: @Override public IFigureStack addFigureStack(IFigureStack stack)
   :outertype: GenericBoardElement

   Adds a figure stack

   :param stack: Stack to be added
   :return: Added stack

addFigureStack
^^^^^^^^^^^^^^

.. java:method:: @Override public IFigureStack addFigureStack(IFigureStack stack, String name)
   :outertype: GenericBoardElement

   Adds a figure stack and assigns a name to it

   :param stack: Stack to be added
   :param name: Assigned name
   :return: Added stack

addFigureStacks
^^^^^^^^^^^^^^^

.. java:method:: @Override public List<IFigureStack> addFigureStacks(List<IFigureStack> stacks)
   :outertype: GenericBoardElement

   Adds lists of figure stacks

   :param stacks: Stack to be added
   :return: Added stack

connectTo
^^^^^^^^^

.. java:method:: @Override public IBoardElement connectTo(IBoardElement target, int cost)
   :outertype: GenericBoardElement

   Connects board elements

   :param target: Target element
   :param cost: Cost in that direction
   :return: Target element

getAllConnectedBoardElements
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public Map<IBoardElement, Integer> getAllConnectedBoardElements()
   :outertype: GenericBoardElement

   Returns all connected board elements

   :return: Connected elements (neighbours)

getAllUnvisitedConnectedElements
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public Map<IBoardElement, Integer> getAllUnvisitedConnectedElements()
   :outertype: GenericBoardElement

   Returns all unvisited but connected elements

   :return: Unvisited neighbours

getDefaultFigure
^^^^^^^^^^^^^^^^

.. java:method:: @Override public IFigure getDefaultFigure()
   :outertype: GenericBoardElement

   Returns the default figure off the default stack

   :return: The default figure if there is a default stack, else null

getDefaultStack
^^^^^^^^^^^^^^^

.. java:method:: @Override public IFigureStack getDefaultStack()
   :outertype: GenericBoardElement

   Returns the default stack (the first element, i.e. with the index of 0)

   :return: Desired stack if it exists, else null

getFigureStacks
^^^^^^^^^^^^^^^

.. java:method:: @Override public IFigureStack getFigureStacks(String name)
   :outertype: GenericBoardElement

   Returns the desired figure stack name-wise

   :param name: Figure name
   :return: Desired stack

getFigureStacks
^^^^^^^^^^^^^^^

.. java:method:: @Override public List<IFigureStack> getFigureStacks()
   :outertype: GenericBoardElement

   Returns the list of figure stacks

   :return: Desired list

getUniqueName
^^^^^^^^^^^^^

.. java:method:: @Override public String getUniqueName()
   :outertype: GenericBoardElement

   Returns the unique name

   :return: Desired unique name

isVisited
^^^^^^^^^

.. java:method:: @Override public boolean isVisited()
   :outertype: GenericBoardElement

   Checks whether an element has been visited

   :return: True if it has, else false

render
^^^^^^

.. java:method:: @Override public void render(Graphics2D g, Point origin, Point extent)
   :outertype: GenericBoardElement

   The renderer draws a board element between originX, originY and originX+extentX and originY+extentY.
   Clipping is not enforced! Rendering is performed by rendering its own visual presenter
   and then calling the render method on all stacks.

   :param g: Graphics element to be drawn on
   :param origin: topLeft coordinate, the starting point for drawing inside g
   :param extent: size of the allocated drawing area, but not limited to it (no clipping)

setUniqueName
^^^^^^^^^^^^^

.. java:method:: @Override public void setUniqueName(String name)
   :outertype: GenericBoardElement

   Assigns a unique name

   :param name: Name of the element

setVisited
^^^^^^^^^^

.. java:method:: @Override public void setVisited(boolean visited)
   :outertype: GenericBoardElement

   Sets the visitation flag

   :param visited: True if it has been visited, else false

