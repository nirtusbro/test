IBoard
======

.. java:package:: Definition
   :noindex:

.. java:type:: public interface IBoard extends IMetadataCore, IRenderable

   Created by hades-incarnate on 10/20/2015. INterface deklaracija zborda koji ce biti implementiran kao povezani graf. Nasledjene varijante tog core baorda mogu da implementiraju specificne boardove kao sto je sahovska tabla.

Methods
-------
addBoardElement
^^^^^^^^^^^^^^^

.. java:method::  IBoardElement addBoardElement(IBoardElement elem)
   :outertype: IBoard

   Dodavanje board elementa

   :param elem: Element koji se dodaje
   :return: Dodati element

addBoardElements
^^^^^^^^^^^^^^^^

.. java:method::  List<IBoardElement> addBoardElements(List<IBoardElement> elems)
   :outertype: IBoard

   Dodavanje liste board elemenata

   :param elems: Lista elemenata koji se dodaju
   :return: Dodate elemente

connectAllElements
^^^^^^^^^^^^^^^^^^

.. java:method::  void connectAllElements(Map<IBoardElement, Map<IBoardElement, Integer>> connectionMap)
   :outertype: IBoard

   Spajanje svih elemenata

   :param connectionMap: Mapa elemenata

connectElements
^^^^^^^^^^^^^^^

.. java:method::  void connectElements(IBoardElement elemStart, IBoardElement elemEnd, int cost)
   :outertype: IBoard

   Spajanje elemenata

   :param elemStart: Pocetak
   :param elemEnd: Kraj
   :param cost: Tezina izmedju njih

connectElements
^^^^^^^^^^^^^^^

.. java:method::  void connectElements(IBoardElement elemStart, IBoardElement elemEnd, int costForward, int costBackward)
   :outertype: IBoard

   Spajanje elemenata sa razlicitim tezinama po smerovima

   :param elemStart: Pocetak
   :param elemEnd: Kraj
   :param costForward: Tezina u smeru pocetak->kraj
   :param costBackward: Tezina u smeru kraj->pocetak

getAllElements
^^^^^^^^^^^^^^

.. java:method::  List<IBoardElement> getAllElements()
   :outertype: IBoard

   Vraca sve elemente grafa

   :return: Lista elemenata

getAllElementsForCost
^^^^^^^^^^^^^^^^^^^^^

.. java:method::  List<IBoardElement> getAllElementsForCost(IBoardElement root, int exactCost)
   :outertype: IBoard

   Pronalazi i vraca sve elemente zadate tezine

   :param root: Koren liste
   :param exactCost: Tezina koja se trazi
   :return: elementi Odredjene tezine

getAllReachableElements
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method::  List<IBoardElement> getAllReachableElements(IBoardElement root, int maxCost)
   :outertype: IBoard

   Nalazi sve spojene elemente

   :param root: Koren liste
   :param maxCost: Najveca tezina
   :return: Sve spojene elemente

getShortestPath
^^^^^^^^^^^^^^^

.. java:method::  List<IBoardElement> getShortestPath(IBoardElement start, IBoardElement target)
   :outertype: IBoard

   Nalazi najkraci put izmedju elemenata

   :param start: Pocetak
   :param target: Cilj
   :return: Najkraci put

