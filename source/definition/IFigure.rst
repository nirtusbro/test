IFigure
=======

.. java:package:: Definition
   :noindex:

.. java:type:: public interface IFigure extends IMetadataCore, IRenderable

   The figure which is used in the game, is renderable.

Methods
-------
getBoard
^^^^^^^^

.. java:method::  IBoard getBoard()
   :outertype: IFigure

   Returns the table on which this figure is on

   :return: The table on which this figure is on

getBoardElement
^^^^^^^^^^^^^^^

.. java:method::  IBoardElement getBoardElement()
   :outertype: IFigure

   Returns the table element on which this figure is on

   :return: The table element on which this figure is on

getFigureStack
^^^^^^^^^^^^^^

.. java:method::  IFigureStack getFigureStack()
   :outertype: IFigure

   Returns the figure stack on which this figure is on

   :return: The figure stack on which this figure is on

getName
^^^^^^^

.. java:method::  String getName()
   :outertype: IFigure

   Returns the figure's name

   :return: Figure name

getOwner
^^^^^^^^

.. java:method::  IPlayer getOwner()
   :outertype: IFigure

   Return the figure's owner

   :return: Figure owner
setName
^^^^^^^

.. java:method::  void setName(String name)
   :outertype: IFigure

   Sets the figure's name

   :param name: Figure name

