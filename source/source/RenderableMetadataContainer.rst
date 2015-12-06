.. java:import:: Definition IRenderable

.. java:import:: Definition IVisualPresentation

RenderableMetadataContainer
===========================

.. java:package:: Source
   :noindex:

.. java:type:: public abstract class RenderableMetadataContainer extends MetadataContainer implements IRenderable

   Created by hades-incarnate on 10/30/2015. implementacija renderable elements

Methods
-------
excludeFromRender
^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void excludeFromRender(boolean exclude)
   :outertype: RenderableMetadataContainer

   A method to omit an element from render cycle

   :param exclude: omit or include element

getVisualPresentation
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public IVisualPresentation getVisualPresentation()
   :outertype: RenderableMetadataContainer

   Returns visual presenter assigned to game object

   :return: presenter

isExcludedFromRender
^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public boolean isExcludedFromRender()
   :outertype: RenderableMetadataContainer

   Indicates whether an element is ommited from main rendering cycle (default false)

   :return: true if element is ommited, false if included.

render
^^^^^^

.. java:method:: @Override public void render(Graphics2D g, Point origin, Point extent)
   :outertype: RenderableMetadataContainer

   render draws between originX, orignY and originX+extentX and originY+extentY. Clipping is not enforced! Rendering is performed by calling render method on visual presenter

   :param g: Graphics element on which to draw
   :param origin: topLeft coordinate from which to draw inside g
   :param extent: size of the allocated drawing area, but not limited to it (no clipping)

setVisualPresentation
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void setVisualPresentation(IVisualPresentation presenter)
   :outertype: RenderableMetadataContainer

   Assigns visual presenter to this game object

   :param presenter: visual presenter

