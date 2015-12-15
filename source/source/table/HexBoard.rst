.. java:import:: javafx.geometry Point3D

.. java:import:: Source.generic GenericBoard

HexBoard
========

.. java:package:: Source.table
   :noindex:

.. java:type:: public class HexBoard extends GenericBoard

Constructors
------------
HexBoard
^^^^^^^^

.. java:constructor:: public HexBoard(Point3D[] points, IBoardElementFactory elementFactory)
   :outertype: HexBoard

   Generating hex table of arbitary shape

HexBoard
^^^^^^^^

.. java:constructor:: public HexBoard(int size, IBoardElementFactory elementFactory)
   :outertype: HexBoard

   Generating hex table hexagonal shape


HexBoard
^^^^^^^^

.. java:constructor:: public HexBoard(int x, int y, layout l, IBoardElementFactory elementFactory)
   :outertype: HexBoard

   Generating hex table square-shaped

HexBoard
^^^^^^^^

.. java:constructor:: public HexBoard(int size, IBoardElementFactory elementFactory, IFigureStacksFactory figureStacksFactory)
   :outertype: HexBoard

HexBoard
^^^^^^^^

.. java:constructor:: public HexBoard(Point3D[] points, IBoardElementFactory elementFactory, IFigureStacksFactory figureStacksFactory)
   :outertype: HexBoard

HexBoard
^^^^^^^^

.. java:constructor:: public HexBoard(int x, int y, layout l, IBoardElementFactory elementFactory, IFigureStacksFactory figureStacksFactory)
   :outertype: HexBoard

Methods
-------
addBoardElement
^^^^^^^^^^^^^^^

.. java:method:: @Override public IBoardElement addBoardElement(IBoardElement elem)
   :outertype: HexBoard

addBoardElements
^^^^^^^^^^^^^^^^

.. java:method:: @Override public List<IBoardElement> addBoardElements(List<IBoardElement> elems)
   :outertype: HexBoard

   Here it returns mistakes because of prohibited methodsds

connectAllElements
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void connectAllElements(Map<IBoardElement, Map<IBoardElement, Integer>> connectionMap)
   :outertype: HexBoard

connectElements
^^^^^^^^^^^^^^^

.. java:method:: @Override public void connectElements(IBoardElement elemStart, IBoardElement elemEnd, int cost)
   :outertype: HexBoard

connectElements
^^^^^^^^^^^^^^^

.. java:method:: @Override public void connectElements(IBoardElement elemStart, IBoardElement elemEnd, int costForward, int costBackward)
   :outertype: HexBoard

getBoardElementAt
^^^^^^^^^^^^^^^^^

.. java:method:: public IBoardElement getBoardElementAt(int x, int y, int z)
   :outertype: HexBoard

getDefaultFigureAt
^^^^^^^^^^^^^^^^^^

.. java:method:: public IFigure getDefaultFigureAt(int x, int y, int z)
   :outertype: HexBoard

