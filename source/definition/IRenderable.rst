IRenderable
===========

.. java:package:: Definition
   :noindex:

.. java:type:: public interface IRenderable

   Created by hades-incorporate on 10/28/2015. This interface defines tight-coupling with IVisualPresentation implementations. Objects implementing inherited interfaces have the ability ro render themselves on screen.

Methods
-------
excludeFromRender
^^^^^^^^^^^^^^^^^

.. java:method::  void excludeFromRender(boolean exclude)
   :outertype: IRenderable

   A method to omit an element from render cycle

   :param exclude: omit or include element

getVisualPresentation
^^^^^^^^^^^^^^^^^^^^^

.. java:method::  IVisualPresentation getVisualPresentation()
   :outertype: IRenderable

   Retrieve visual presenter for this renderable element

   :return: visual presenter

isExcludedFromRender
^^^^^^^^^^^^^^^^^^^^

.. java:method::  boolean isExcludedFromRender()
   :outertype: IRenderable

   Indicates whether an element is ommited from main rendering cycle (default false)

   :return: true if element is ommited, false if included.

render
^^^^^^

.. java:method::  void render(Graphics2D g, Point origin, Point extent)
   :outertype: IRenderable

   render draws between originX, orignY and originX+extentX and originY+extentY. Clipping is not enforced!

   :param g: Graphics element on which to draw
   :param origin: topLeft coordinate from which to draw inside g
   :param extent: size of the allocated drawing area, but not limited to it (no clipping)

setVisualPresentation
^^^^^^^^^^^^^^^^^^^^^

.. java:method::  void setVisualPresentation(IVisualPresentation presenter)
   :outertype: IRenderable

   Retrieve visual presenter for this renderable element

   :param presenter: visual presenter

