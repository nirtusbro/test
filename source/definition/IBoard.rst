IBoard
======

.. java:package:: Definition
   :noindex:

.. java:type:: public interface IBoard extends IMetadataCore, IRenderable

   Interface declaration of Board which is implemented as a connected graph.
   
Methods
-------
addBoardElement
^^^^^^^^^^^^^^^

.. java:method::  IBoardElement addBoardElement(IBoardElement elem)
   :outertype: IBoard

   Adds a board element

   :param elem: Element to be added
   :return: Added element

addBoardElements
^^^^^^^^^^^^^^^^

.. java:method::  List<IBoardElement> addBoardElements(List<IBoardElement> elems)
   :outertype: IBoard
   
   Adds a list of board elements

   :param elems: A list of elements to be added
   :return: Added elements

connectAllElements
^^^^^^^^^^^^^^^^^^

.. java:method::  void connectAllElements(Map<IBoardElement, Map<IBoardElement, Integer>> connectionMap)
   :outertype: IBoard

   Connects all elements

   :param connectionMap: A map of elements

connectElements
^^^^^^^^^^^^^^^

.. java:method::  void connectElements(IBoardElement elemStart, IBoardElement elemEnd, int cost)
   :outertype: IBoard

   Connects elements

   :param elemStart: First element
   :param elemEnd: Last element
   :param cost: The cost between them

connectElements
^^^^^^^^^^^^^^^

.. java:method::  void connectElements(IBoardElement elemStart, IBoardElement elemEnd, int costForward, int costBackward)
   :outertype: IBoard

   Connecting elements with different costs depending on the direction

   :param elemStart: Starting element
   :param elemEnd: Ending
   :param costForward: Cost in the beggining->end direction
   :param costBackward: Cost in the end->beggining direction

getAllElements
^^^^^^^^^^^^^^

.. java:method::  List<IBoardElement> getAllElements()
   :outertype: IBoard

   Returns all the elements of the graph

   :return: A list of elements

getAllElementsForCost
^^^^^^^^^^^^^^^^^^^^^

.. java:method::  List<IBoardElement> getAllElementsForCost(IBoardElement root, int exactCost)
   :outertype: IBoard

   Pronalazi i vraca sve elemente zadate tezine
   Looks for and returns all elements of a given cost

   :param root: The list's root element
   :param exactCost: The given cost
   :return: A list of elements of a given cost

getAllReachableElements
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method::  List<IBoardElement> getAllReachableElements(IBoardElement root, int maxCost)
   :outertype: IBoard

   Looks for all connected elements

   :param root: The list's root element
   :param maxCost: Maximum cost
   :return: A list of elements that are connected

getShortestPath
^^^^^^^^^^^^^^^

.. java:method::  List<IBoardElement> getShortestPath(IBoardElement start, IBoardElement target)
   :outertype: IBoard

   Looks for the shortest path between two elements

   :param start: First element
   :param target: Last element
   :return: The shortest path

