.. java:import:: Source RenderableMetadataContainer

.. java:import:: java.util List

.. java:import:: java.util.stream Collectors

GenericBoardElement
===================

.. java:package:: Source.generic
   :noindex:

.. java:type:: public class GenericBoardElement extends RenderableMetadataContainer implements IBoardElement

   Created by Filip Comor on 31-Oct-15. Genericki board element

Constructors
------------
GenericBoardElement
^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public GenericBoardElement(IBoard board)
   :outertype: GenericBoardElement

Methods
-------
addFigureStack
^^^^^^^^^^^^^^

.. java:method:: @Override public IFigureStack addFigureStack(IFigureStack stack)
   :outertype: GenericBoardElement

   Dodaje steka figura

   :param stack: Stek koji se dodaje
   :return: Dodati stek

addFigureStack
^^^^^^^^^^^^^^

.. java:method:: @Override public IFigureStack addFigureStack(IFigureStack stack, String name)
   :outertype: GenericBoardElement

   Dodaje stek i zadaje mu ime

   :param stack: Stek koji se dodaje
   :param name: Zadato ime
   :return: Dodati stek

addFigureStacks
^^^^^^^^^^^^^^^

.. java:method:: @Override public List<IFigureStack> addFigureStacks(List<IFigureStack> stacks)
   :outertype: GenericBoardElement

   Dodaje liste stekova figura

   :param stacks: Stek koji se dodaje
   :return: Dodati stek

connectTo
^^^^^^^^^

.. java:method:: @Override public IBoardElement connectTo(IBoardElement target, int cost)
   :outertype: GenericBoardElement

   Spaja bord elemente

   :param target: Odrediste veze
   :param cost: Trosak u tom smeru
   :return: Ciljni element

getAllConnectedBoardElements
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public Map<IBoardElement, Integer> getAllConnectedBoardElements()
   :outertype: GenericBoardElement

   Geter za sve spojene bord elemente

   :return: Trazene susede, tj. spojene

getAllUnvisitedConnectedElements
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public Map<IBoardElement, Integer> getAllUnvisitedConnectedElements()
   :outertype: GenericBoardElement

   Geter za sve neposecene a spojene bord elemente

   :return: Trazene elemente, tj. susede i neposecene

getDefaultFigure
^^^^^^^^^^^^^^^^

.. java:method:: @Override public IFigure getDefaultFigure()
   :outertype: GenericBoardElement

   Geter default figure sa default steka

   :return: Vraca default figuru ako default stek postoji, inace null

getDefaultStack
^^^^^^^^^^^^^^^

.. java:method:: @Override public IFigureStack getDefaultStack()
   :outertype: GenericBoardElement

   Geter default steka (prvi element, index 0)

   :return: Trazeni stack ako postoji, inace null

getFigureStacks
^^^^^^^^^^^^^^^

.. java:method:: @Override public IFigureStack getFigureStacks(String name)
   :outertype: GenericBoardElement

   Vraca trazeni stek po imenu

   :param name: Naziv figure
   :return: Trazeni stek

getFigureStacks
^^^^^^^^^^^^^^^

.. java:method:: @Override public List<IFigureStack> getFigureStacks()
   :outertype: GenericBoardElement

   Geter za listu stekova figura

   :return: Trazenu listu

getUniqueName
^^^^^^^^^^^^^

.. java:method:: @Override public String getUniqueName()
   :outertype: GenericBoardElement

   Geter za jedinstveno ime

   :return: Vraca trazeno ime

isVisited
^^^^^^^^^

.. java:method:: @Override public boolean isVisited()
   :outertype: GenericBoardElement

   Proverava da li je posecen bord element

   :return: False ako nije, inace true

render
^^^^^^

.. java:method:: @Override public void render(Graphics2D g, Point origin, Point extent)
   :outertype: GenericBoardElement

   render draws board element between originX, orignY and originX+extentX and originY+extentY. Clipping is not enforced! Rendering is performed by rendering its own visual presenter and then calling render method on all stacks

   :param g: Graphics element on which to draw
   :param origin: topLeft coordinate from which to draw inside g
   :param extent: size of the allocated drawing area, but not limited to it (no clipping)

setUniqueName
^^^^^^^^^^^^^

.. java:method:: @Override public void setUniqueName(String name)
   :outertype: GenericBoardElement

   Zadaje jedinstveno ime

   :param name: Ime board elementa

setVisited
^^^^^^^^^^

.. java:method:: @Override public void setVisited(boolean visited)
   :outertype: GenericBoardElement

   Postavlja flag posecenosti

   :param visited: False ako nije, inace true

