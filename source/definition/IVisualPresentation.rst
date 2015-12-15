.. java:import:: java.util List

.. java:import:: java.util NoSuchElementException

IVisualPresentation
===================

.. java:package:: Definition
   :noindex:

.. java:type:: public interface IVisualPresentation

   This interface abstracts visual presentation from the semantics of game elements. As such, it does not define nor enforce rendering methods (shape, image, etc) and can be hooked on different game elements (board, board element, stack, figure, etc). All that is expected from visual presentation is to be able to render itself in a designated area using supplied Java2D graphics object. There should be several implementations of this interface (bitmap, etc)

Methods
-------
addChildPresenters
^^^^^^^^^^^^^^^^^^

.. java:method::  void addChildPresenters(IVisualPresentation presenter)
   :outertype: IVisualPresentation

   Support for composite presenters. Add child presenter

   :param presenter: new child visual presenter

getChildPresenters
^^^^^^^^^^^^^^^^^^

.. java:method::  List<IVisualPresentation> getChildPresenters()
   :outertype: IVisualPresentation

   Support for composite presenters. Return all child presenters

   :return: A list of child visual presenters

removeChildPresenters
^^^^^^^^^^^^^^^^^^^^^

.. java:method::  void removeChildPresenters(IVisualPresentation presenter) throws NoSuchElementException
   :outertype: IVisualPresentation

   Support for composite presenters. Remove child presenter

   :param presenter: existing child presenter to remove

render
^^^^^^

.. java:method::  void render(Graphics2D g, Point origin, Point extent)
   :outertype: IVisualPresentation

   Renders presentation between originX, orignY and originX+extentX and originY+extentY. Clipping is not enforced, so oversized presentations are allowed.

   :param g: Graphics element on which to draw
   :param origin: topLeft coordinate from which to draw inside g
   :param extent: size of the allocated drawing area, but not limited to it (no clipping)

