.. java:import:: Source.generic GenericBoard

.. java:import:: java.awt Point

TableBoard
==========

.. java:package:: Source.table
   :noindex:

.. java:type:: public class TableBoard extends GenericBoard

   Created by hades-incarnate on 10/30/2015. Osnova za XxY tabele (sah, XO, itd)

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

   Ovde vraca greske zbog zabranjenih metoda

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

   Geter za bord element na odredjenoj poziciji

   :param row: Trazeni red
   :param col: Trazena kolona
   :return: Trazeni element

getDefaultFigureAt
^^^^^^^^^^^^^^^^^^

.. java:method:: public IFigure getDefaultFigureAt(int row, int col)
   :outertype: TableBoard

   Geter za default figuru na odredjenoj poziciji

   :param row: Trazeni red
   :param col: Trazena koona
   :return: Trazena figura

