.. java:import:: java.util List

IFigureStack
============

.. java:package:: Definition
   :noindex:

.. java:type:: public interface IFigureStack extends IMetadataCore, IRenderable

   Created by hades-incarnate on 10/20/2015. jedan board element moze da ima vise stackova na razlicitim lokacijama, stack definise oblast i poredak figura, pri cemu se figure renderuju po internom redosledu (sortable?)

Methods
-------
addFigure
^^^^^^^^^

.. java:method::  IFigure addFigure(IFigure figure, String name)
   :outertype: IFigureStack

   Dodavanje figure u listu

   :param figure: Figura koja se dodaje
   :param name: Ime figure koja se dodaje
   :return: Dodatu figuru

addFigures
^^^^^^^^^^

.. java:method::  List<IFigure> addFigures(List<IFigure> figures)
   :outertype: IFigureStack

   Dodavanje liste figura u listu

   :param figures: Lista figura koja se dodaje
   :return: dodate Figure

getDefaultFigure
^^^^^^^^^^^^^^^^

.. java:method::  IFigure getDefaultFigure()
   :outertype: IFigureStack

   Vraca default figuru iz stacka, null ako ja nema Pod default figure se podrazumeva prvo kreirana figura na stacku. Ovo ce nam pomagati kod igrica koje imaju samo jedan stack i jednu figuru po board elementu (npr sah)

   :return: Osnovna figura

getFigure
^^^^^^^^^

.. java:method::  IFigure getFigure(String name)
   :outertype: IFigureStack

   Uzimanje figure iz liste

   :param name: Ime trazene figure
   :return: Trazenu figuru

getFigures
^^^^^^^^^^

.. java:method::  List<IFigure> getFigures()
   :outertype: IFigureStack

   Vraca figura iz liste

   :return: Trazene figure

getName
^^^^^^^

.. java:method::  String getName()
   :outertype: IFigureStack

   Funkcija koja vraca ime figure

   :return: Ime figure

hasFigures
^^^^^^^^^^

.. java:method::  boolean hasFigures()
   :outertype: IFigureStack

   Da li sadrzi figure

   :return: False ako nije prazno

setName
^^^^^^^

.. java:method::  void setName(String name)
   :outertype: IFigureStack

   Funkcija za postavljanje imena figure

   :param name: Ime figure

