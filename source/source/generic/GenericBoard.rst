.. java:import:: Source RenderableMetadataContainer

.. java:import:: java.util List

GenericBoard
============

.. java:package:: Source.generic
   :noindex:

.. java:type:: public class GenericBoard extends RenderableMetadataContainer implements IBoard

   Generic board implementation using graphs

Constructors
------------
GenericBoard
^^^^^^^^^^^^

.. java:constructor:: public GenericBoard()
   :outertype: GenericBoard

   Constructor

Methods
-------
addBoardElement
^^^^^^^^^^^^^^^

.. java:method:: @Override public IBoardElement addBoardElement(IBoardElement elem)
   :outertype: GenericBoard

   Adds a board element

   :param elem: Element to be added
   :return: Added element

addBoardElements
^^^^^^^^^^^^^^^^

.. java:method:: @Override public List<IBoardElement> addBoardElements(List<IBoardElement> elems)
   :outertype: GenericBoard

   Adds a list of board elements

   :param elems: List of elements to be added
   :return: Added elements

connectAllElements
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void connectAllElements(Map<IBoardElement, Map<IBoardElement, Integer>> connectionMap)
   :outertype: GenericBoard

   Connects all elements

   :param connectionMap: Map of the elements

connectElements
^^^^^^^^^^^^^^^

.. java:method:: @Override public void connectElements(IBoardElement elemStart, IBoardElement elemEnd, int cost)
   :outertype: GenericBoard

   Connects desired elements

   :param elemStart: Starting element
   :param elemEnd: Ending element
   :param cost: Cost between them

connectElements
^^^^^^^^^^^^^^^

.. java:method:: @Override public void connectElements(IBoardElement elemStart, IBoardElement elemEnd, int costForward, int costBackward)
   :outertype: GenericBoard

   Connects elements with different costs direction-wise

   :param elemStart: Starting element
   :param elemEnd: Ending element
   :param costForward: Cost in the start->end direction
   :param costBackward: Cost in the end->start direction

getAllElements
^^^^^^^^^^^^^^

.. java:method:: @Override public List<IBoardElement> getAllElements()
   :outertype: GenericBoard

   Returns all elements from the graph

   :return: List of elements

getAllElementsForCost
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public List<IBoardElement> getAllElementsForCost(IBoardElement root, int exactCost)
   :outertype: GenericBoard

   Finds and returns all elements with the given cost

   :param root: Board element list root
   :param exactCost: Desired cost value
   :return: Elements with the desired cost value

getAllReachableElements
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public List<IBoardElement> getAllReachableElements(IBoardElement start, int maxCost)
   :outertype: GenericBoard

   Finds all connected elements

   :param start: Board element list root
   :param maxCost: Maximum cost
   :return: All connected elements

getShortestPath
^^^^^^^^^^^^^^^

.. java:method:: @Override public List<IBoardElement> getShortestPath(IBoardElement start, IBoardElement target)
   :outertype: GenericBoard

   Finds the shortest path between two given elements

   :param start: Starting element
   :param target: Target element
   :return: Shortest path

render
^^^^^^

.. java:method:: @Override public void render(Graphics2D g, Point origin, Point extent)
   :outertype: GenericBoard

   The renderer draws a board element between originX, originY and originX+extentX and originY+extentY.
   Clipping is not enforced! Rendering is performed by rendering its own visual presenter
   and then calling the render method on all board elements.

   :param g: Graphics element to be drawn on
   :param origin: topLeft coordinate, the starting point for drawing inside g
   :param extent: size of the allocated drawing area, but not limited to it (no clipping)

