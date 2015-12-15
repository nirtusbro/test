.. java:import:: Source.generic GenericBoard

.. java:import:: java.awt Point

TableBoard
==========

.. java:package:: Source.table
   :noindex:

.. java:type:: public class TableBoard extends GenericBoard

   Basis for XxY tables(sah, XO, etc)

Constructors
------------
TableBoard
^^^^^^^^^^

.. java:constructor:: public TableBoard(int cols, int rows, IBoardElementFactory elementFactory)
   :outertype: TableBoard

TableBoard
^^^^^^^^^^

.. java:constructor:: public TableBoard(int cols, int rows, IBoardElementFactory elementFactory, IFigureStacksFactory figureStacksFactory)
   :outertype: TableBoard

Methods
-------
addBoardElement
^^^^^^^^^^^^^^^

.. java:method:: @Override public IBoardElement addBoardElement(IBoardElement elem)
   :outertype: TableBoard

addBoardElements
^^^^^^^^^^^^^^^^

.. java:method:: @Override public List<IBoardElement> addBoardElements(List<IBoardElement> elems)
   :outertype: TableBoard

    Here it returns mistakes because of prohibited methodsds

connectAllElements
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void connectAllElements(Map<IBoardElement, Map<IBoardElement, Integer>> connectionMap)
   :outertype: TableBoard

connectElements
^^^^^^^^^^^^^^^

.. java:method:: @Override public void connectElements(IBoardElement elemStart, IBoardElement elemEnd, int cost)
   :outertype: TableBoard

connectElements
^^^^^^^^^^^^^^^

.. java:method:: @Override public void connectElements(IBoardElement elemStart, IBoardElement elemEnd, int costForward, int costBackward)
   :outertype: TableBoard

getBoardElementAt
^^^^^^^^^^^^^^^^^

.. java:method:: public IBoardElement getBoardElementAt(int row, int col)
   :outertype: TableBoard

  Getter for board elements on certain position

   :param row: Wanted row
   :param col: Wanted column
   :return: Wanted element

getDefaultFigureAt
^^^^^^^^^^^^^^^^^^

.. java:method:: public IFigure getDefaultFigureAt(int row, int col)
   :outertype: TableBoard

  Getter for default figure on certain position

   :param row: Wanted row
   :param col: Wanted column
   :return: Wanted figure

