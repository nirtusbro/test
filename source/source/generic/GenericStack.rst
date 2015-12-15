.. java:import:: Source RenderableMetadataContainer

.. java:import:: java.util ArrayList

.. java:import:: java.util List

GenericStack
============

.. java:package:: Source.generic
   :noindex:

.. java:type:: public class GenericStack extends RenderableMetadataContainer implements IFigureStack

   Generic figure stack

Methods
-------
addFigure
^^^^^^^^^

.. java:method:: @Override public IFigure addFigure(IFigure figure, String name)
   :outertype: GenericStack

   Adds a figure

   :param figure: Figure to be added
   :param name: Name of said figure
   :return: Added figure

addFigures
^^^^^^^^^^

.. java:method:: @Override public List<IFigure> addFigures(List<IFigure> figures)
   :outertype: GenericStack

   Adds a list of figures

   :param figures: Figure list to be added
   :return: Added figures

getDefaultFigure
^^^^^^^^^^^^^^^^

.. java:method:: @Override public IFigure getDefaultFigure()
   :outertype: GenericStack

   Returns the default figure

   :return: Default figure

getFigure
^^^^^^^^^

.. java:method:: @Override public IFigure getFigure(String name)
   :outertype: GenericStack

   Returns the desired figure by name

   :param name: Name of desired figure
   :return: Desired figure

getFigures
^^^^^^^^^^

.. java:method:: @Override public List<IFigure> getFigures()
   :outertype: GenericStack

   Returns figures from a list

   :return: Desired figures

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: GenericStack

   Returns the name of the desired stack

   :return: Stack name

hasFigures
^^^^^^^^^^

.. java:method:: @Override public boolean hasFigures()
   :outertype: GenericStack

   Checks whether a stack contains any figures

   :return: True if yes, else false

render
^^^^^^

.. java:method:: @Override public void render(Graphics2D g, Point origin, Point extent)
   :outertype: GenericStack

   The renderer draws a stack between originX, originY and originX+extentX and originY+extentY.
   Clipping is not enforced! Rendering is performed by rendering its own visual presenter
   and then calling the render method on all figures

   :param g: Graphics element to be drawn on
   :param origin: topLeft coordinate, the starting point for drawing inside g
   :param extent: size of the allocated drawing area, but not limited to it (no clipping)

setName
^^^^^^^

.. java:method:: @Override public void setName(String name)
   :outertype: GenericStack

    Sets the name of the desired figure

    :param name: Desired name