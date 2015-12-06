.. java:import:: Source RenderableMetadataContainer

.. java:import:: java.util List

GenericBoard
============

.. java:package:: Source.generic
   :noindex:

.. java:type:: public class GenericBoard extends RenderableMetadataContainer implements IBoard

   Created by hades-incarnate on 10/30/2015. Generic board implementation using graphs

Constructors
------------
GenericBoard
^^^^^^^^^^^^

.. java:constructor:: public GenericBoard()
   :outertype: GenericBoard

   Konstruktor

Methods
-------
addBoardElement
^^^^^^^^^^^^^^^

.. java:method:: @Override public IBoardElement addBoardElement(IBoardElement elem)
   :outertype: GenericBoard

   Dodavanje board elementa

   :param elem: Element koji se dodaje
   :return: Dodati element

addBoardElements
^^^^^^^^^^^^^^^^

.. java:method:: @Override public List<IBoardElement> addBoardElements(List<IBoardElement> elems)
   :outertype: GenericBoard

   Dodavanje liste board elemenata

   :param elems: Lista elemenata koji se dodaju
   :return: Dodate elemente

connectAllElements
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void connectAllElements(Map<IBoardElement, Map<IBoardElement, Integer>> connectionMap)
   :outertype: GenericBoard

   Spajanje svih elemenata

   :param connectionMap: Mapa elemenata

connectElements
^^^^^^^^^^^^^^^

.. java:method:: @Override public void connectElements(IBoardElement elemStart, IBoardElement elemEnd, int cost)
   :outertype: GenericBoard

   Spajanje elemenata

   :param elemStart: Pocetak
   :param elemEnd: Kraj
   :param cost: Tezina izmedju njih

connectElements
^^^^^^^^^^^^^^^

.. java:method:: @Override public void connectElements(IBoardElement elemStart, IBoardElement elemEnd, int costForward, int costBackward)
   :outertype: GenericBoard

   Spajanje elemenata sa razlicitim tezinama po smerovima

   :param elemStart: Pocetak
   :param elemEnd: Kraj
   :param costForward: Tezina u smeru pocetak->kraj
   :param costBackward: Tezina u smeru kraj->pocetak

getAllElements
^^^^^^^^^^^^^^

.. java:method:: @Override public List<IBoardElement> getAllElements()
   :outertype: GenericBoard

   Vraca sve elemente grafa

   :return: Lista elemenata

getAllElementsForCost
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public List<IBoardElement> getAllElementsForCost(IBoardElement root, int exactCost)
   :outertype: GenericBoard

   Pronalazi i vraca sve elemente zadate tezine

   :param root: Koren liste
   :param exactCost: Tezina koja se trazi
   :return: Elementi odredjene tezine

getAllReachableElements
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public List<IBoardElement> getAllReachableElements(IBoardElement start, int maxCost)
   :outertype: GenericBoard

   Nalazi sve spojene elemente

   :param start: Koren liste
   :param maxCost: Najveca tezina
   :return: Sve spojene elemente

getShortestPath
^^^^^^^^^^^^^^^

.. java:method:: @Override public List<IBoardElement> getShortestPath(IBoardElement start, IBoardElement target)
   :outertype: GenericBoard

   Nalazi najkraci put izmedju elemenata

   :param start: Pocetak
   :param target: Cilj
   :return: Najkraci put

render
^^^^^^

.. java:method:: @Override public void render(Graphics2D g, Point origin, Point extent)
   :outertype: GenericBoard

   render draws board element between originX, orignY and originX+extentX and originY+extentY. Clipping is not enforced! Rendering is performed by rendering its own visual presenter and then calling render method on all board elements

   :param g: Graphics element on which to draw
   :param origin: topLeft coordinate from which to draw inside g
   :param extent: size of the allocated drawing area, but not limited to it (no clipping)

