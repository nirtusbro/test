.. java:import:: Source RenderableMetadataContainer

GenericFigure
=============

.. java:package:: Source.generic
   :noindex:

.. java:type:: public class GenericFigure extends RenderableMetadataContainer implements IFigure

   Created by hades-incarnate on 10/30/2015. Genericka figura koju ce nasledjivati sve buduce figure

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

   Konstruktor genericke figure

   :param name: Ime figure
   :param player: Vlasnik figure
   :param figureStack: Stek figura na kome se nalazi figura
   :param boardElement: Element table na kome se nalazi figura
   :param board: Tabla na kojoj se nalazi figura

Methods
-------
getBoard
^^^^^^^^

.. java:method:: @Override public IBoard getBoard()
   :outertype: GenericFigure

   Vraca tablu na kojoj se nalazi figura

   :return: Tabla na kojoj se nalazi figura

getBoardElement
^^^^^^^^^^^^^^^

.. java:method:: @Override public IBoardElement getBoardElement()
   :outertype: GenericFigure

   Vraca element table na kojoj se trenutno nalazi figura

   :return: Element table na kojoj se trenutno nalazi figura

getFigureStack
^^^^^^^^^^^^^^

.. java:method:: @Override public IFigureStack getFigureStack()
   :outertype: GenericFigure

   Vraca stek figura na kome se nalazi figura

   :return: Stek figura na kome se nalazi figura

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: GenericFigure

   Vraca ime figure

   :return: Ime figure

getOwner
^^^^^^^^

.. java:method:: @Override public IPlayer getOwner()
   :outertype: GenericFigure

   Vraca vlasnika figure

   :return: Vlasnik figure

setName
^^^^^^^

.. java:method:: @Override public void setName(String name)
   :outertype: GenericFigure

   Postavlja ime figure

   :param name: Ime figure

