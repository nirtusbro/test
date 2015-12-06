IBoardElement
=============

.. java:package:: Definition
   :noindex:

.. java:type:: public interface IBoardElement extends IMetadataCore, IRenderable

   Created by hades-incarnate on 10/20/2015. Jedan element board-a, renderable i sadrzi vise stackova figura

Methods
-------
addFigureStack
^^^^^^^^^^^^^^

.. java:method::  IFigureStack addFigureStack(IFigureStack stack)
   :outertype: IBoardElement

addFigureStack
^^^^^^^^^^^^^^

.. java:method::  IFigureStack addFigureStack(IFigureStack stack, String name)
   :outertype: IBoardElement

   Dodaje stek figura

   :param stack: Stek na koji se dodaje
   :param name: Ime steka
   :return: Stek koji se dodaje

addFigureStacks
^^^^^^^^^^^^^^^

.. java:method::  List<IFigureStack> addFigureStacks(List<IFigureStack> stacks)
   :outertype: IBoardElement

connectTo
^^^^^^^^^

.. java:method::  IBoardElement connectTo(IBoardElement target, int cost)
   :outertype: IBoardElement

   Povezuje ovaj board element sa drugim

   :param target: Odrediste veze
   :param cost: Trosak u tom smeru
   :return: vraca sebe, radi ulancavanje connectTo() poziva

getAllConnectedBoardElements
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method::  Map<IBoardElement, Integer> getAllConnectedBoardElements()
   :outertype: IBoardElement

   Svi board elementi koji su povezani za ovaj u smeru ovaj->drugi

   :return: Mapa povezanih elemenata i tezine puteva

getAllUnvisitedConnectedElements
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method::  Map<IBoardElement, Integer> getAllUnvisitedConnectedElements()
   :outertype: IBoardElement

   Pomoc za algoritme pretrage, vrati samo one povezane elemente gde je !isVisited()

   :return: Mapa neposecenih povezanih elemenata i tezine puteva

getDefaultFigure
^^^^^^^^^^^^^^^^

.. java:method::  IFigure getDefaultFigure()
   :outertype: IBoardElement

   Vraca default figuru iz elementa, null ako ga nema ili element nema stackova. Pod default stack se podrazumeva prvo kreirana figura na prvo kreiranom stacku. Ovo ce nam pomagati kod igrica koje imaju samo jedan stack i jednu figuru po board elementu (npr sah)

   :return: Osnovna figura

getDefaultStack
^^^^^^^^^^^^^^^

.. java:method::  IFigureStack getDefaultStack()
   :outertype: IBoardElement

   Vraca default stack iz elementa, null ako ga nema. Pod default stack se podrazumeva prvo kreirani stack. Ovo ce nam pomagati kod igrica koje imaju samo jedan stack po board elementu

   :return: Osnovni figure stack

getFigureStacks
^^^^^^^^^^^^^^^

.. java:method::  List<IFigureStack> getFigureStacks()
   :outertype: IBoardElement

   Vraca stekove figura

   :return: Stekovi figura

getFigureStacks
^^^^^^^^^^^^^^^

.. java:method::  IFigureStack getFigureStacks(String name)
   :outertype: IBoardElement

   Vraca stek figura sa zadatim nazivom

   :param name: Naziv figure
   :return: Stek figura

getUniqueName
^^^^^^^^^^^^^

.. java:method::  String getUniqueName()
   :outertype: IBoardElement

   Vraca jedinstveno ime

   :return: Ime board elementa

isVisited
^^^^^^^^^

.. java:method::  boolean isVisited()
   :outertype: IBoardElement

   Vraca da li je element posecen

   :return: false ako nije, true ako jeste

setUniqueName
^^^^^^^^^^^^^

.. java:method::  void setUniqueName(String name)
   :outertype: IBoardElement

   Postavlja jedinstveno ime board elementa. Pozeljno bi bilo da IBoard.addBoardElement validira jedistvenost

   :param name: Ime board elementa

setVisited
^^^^^^^^^^

.. java:method::  void setVisited(boolean visited)
   :outertype: IBoardElement

   Obelezava da li je element posecen

   :param visited: false ako nije, true ako jeste

