.. java:import:: Source RenderableMetadataContainer

GenericFigure
=============

.. java:package:: Source.generic
   :noindex:

.. java:type:: public class GenericFigure extends RenderableMetadataContainer implements IFigure

   Generic figure

Constructors
------------
GenericFigure
^^^^^^^^^^^^^

.. java:constructor:: public GenericFigure()
   :outertype: GenericFigure

GenericFigure
^^^^^^^^^^^^^

.. java:constructor:: public GenericFigure(String name, IPlayer player, IFigureStack figureStack, IBoardElement boardElement, IBoard board)
   :outertype: GenericFigure

   Generic figure constructor

   :param name: Name of the figure
   :param player: Owner of the figure
   :param figureStack: Figure stack to which this figure belongs to
   :param boardElement: Board element where this figure is placed
   :param board: The board where this figure is placed

Methods
-------
getBoard
^^^^^^^^

.. java:method:: @Override public IBoard getBoard()
   :outertype: GenericFigure

   Returns the board which contains this figure

   :return: Desired board

getBoardElement
^^^^^^^^^^^^^^^

.. java:method:: @Override public IBoardElement getBoardElement()
   :outertype: GenericFigure

   Returns the board element which contains this figure

   :return: Board element which contains this figure

getFigureStack
^^^^^^^^^^^^^^

.. java:method:: @Override public IFigureStack getFigureStack()
   :outertype: GenericFigure

   Returns the figure stack which contains this figure

   :return: Figure stack which contains this figure

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: GenericFigure

   Returns the figure name

   :return: Figure name

getOwner
^^^^^^^^

.. java:method:: @Override public IPlayer getOwner()
   :outertype: GenericFigure

   Returns the owner of this figure

   :return: Owner of this figure

setName
^^^^^^^

.. java:method:: @Override public void setName(String name)
   :outertype: GenericFigure

   Sets the desired name of the figure

   :param name: Name of the figure

