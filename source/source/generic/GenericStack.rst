.. java:import:: Source RenderableMetadataContainer

.. java:import:: java.util ArrayList

.. java:import:: java.util List

GenericStack
============

.. java:package:: Source.generic
   :noindex:

.. java:type:: public class GenericStack extends RenderableMetadataContainer implements IFigureStack

   Created by djura on 31-Oct-15. Genericki stack figura kog ce nasledjivati svi buduci stackovi

Methods
-------
addFigure
^^^^^^^^^

.. java:method:: @Override public IFigure addFigure(IFigure figure, String name)
   :outertype: GenericStack

   Dodavanje figure u listu

   :param figure: Figura koja se dodaje
   :param name: Ime figure koja se dodaje
   :return: Dodatu figuru

addFigures
^^^^^^^^^^

.. java:method:: @Override public List<IFigure> addFigures(List<IFigure> figures)
   :outertype: GenericStack

   Dodavanje liste figura u listu

   :param figures: Lista figura koja se dodaje
   :return: dodate Figure

getDefaultFigure
^^^^^^^^^^^^^^^^

.. java:method:: @Override public IFigure getDefaultFigure()
   :outertype: GenericStack

getFigure
^^^^^^^^^

.. java:method:: @Override public IFigure getFigure(String name)
   :outertype: GenericStack

   Uzimanje figure iz liste

   :param name: Ime trazene figure
   :return: Trazenu figuru

getFigures
^^^^^^^^^^

.. java:method:: @Override public List<IFigure> getFigures()
   :outertype: GenericStack

   Vraca figura iz liste

   :return: Trazene figure

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: GenericStack

hasFigures
^^^^^^^^^^

.. java:method:: @Override public boolean hasFigures()
   :outertype: GenericStack

   Da li sadrzi figure

   :return: False ako nije prazno

render
^^^^^^

.. java:method:: @Override public void render(Graphics2D g, Point origin, Point extent)
   :outertype: GenericStack

   render draws stack between originX, orignY and originX+extentX and originY+extentY. Clipping is not enforced! Rendering is performed by rendering its own visual presenter and then calling render method on all figures

   :param g: Graphics element on which to draw
   :param origin: topLeft coordinate from which to draw inside g
   :param extent: size of the allocated drawing area, but not limited to it (no clipping)

setName
^^^^^^^

.. java:method:: @Override public void setName(String name)
   :outertype: GenericStack

