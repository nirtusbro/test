IFigure
=======

.. java:package:: Definition
   :noindex:

.. java:type:: public interface IFigure extends IMetadataCore, IRenderable

   Created by hades-incarnate on 10/20/2015. Figura koja se pomera u igri, renderable

Methods
-------
getBoard
^^^^^^^^

.. java:method::  IBoard getBoard()
   :outertype: IFigure

   Funkcija koja vraca tablu na kojoj se nalazi figura

   :return: Tabla na kojoj se nalazi figura

getBoardElement
^^^^^^^^^^^^^^^

.. java:method::  IBoardElement getBoardElement()
   :outertype: IFigure

   Funkcija koja vraca element table na kojoj se trenutno nalazi figura

   :return: Element table na kojoj se trenutno nalazi figura

getFigureStack
^^^^^^^^^^^^^^

.. java:method::  IFigureStack getFigureStack()
   :outertype: IFigure

   Funkcija koja vraca stek figura na kome se nalazi figura

   :return: Stek figura na kome se nalazi figura

getName
^^^^^^^

.. java:method::  String getName()
   :outertype: IFigure

   Funkcija koja vraca ime figure

   :return: Ime figure

getOwner
^^^^^^^^

.. java:method::  IPlayer getOwner()
   :outertype: IFigure

   Funkcija koja vraca vlasnika figure

   :return: Vlasnik figure

setName
^^^^^^^

.. java:method::  void setName(String name)
   :outertype: IFigure

   Funkcija za postavljanje imena figure

   :param name: Ime figure

