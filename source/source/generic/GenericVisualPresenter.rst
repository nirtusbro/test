.. java:import:: Definition IVisualPresentation

.. java:import:: java.util List

GenericVisualPresenter
======================

.. java:package:: Source.generic
   :noindex:

.. java:type:: public abstract class GenericVisualPresenter implements IVisualPresentation

   Basic, non-composite visual presenter, hiding the composite implementation,
   should be inherited by simple one-stop presenters

Methods
-------
addChildPresenters
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public final void addChildPresenters(IVisualPresentation presenter)
   :outertype: GenericVisualPresenter

   Add child presenter is disabled. Use CompositeVisualPresenter for this

   :param presenter: not used

getChildPresenters
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public final List<IVisualPresentation> getChildPresenters()
   :outertype: GenericVisualPresenter

   Returns null as child presenters. Use CompositeVisualPresenter for this

   :return: null

removeChildPresenters
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public final void removeChildPresenters(IVisualPresentation presenter) throws NoSuchElementException
   :outertype: GenericVisualPresenter

   Remove child presenter is disabled. Use CompositeVisualPresenter for this. Always throws NoSuchElementException

   :param presenter: not used

render
^^^^^^

.. java:method:: @Override public abstract void render(Graphics2D g, Point origin, Point extent)
   :outertype: GenericVisualPresenter

   Abstract method to render presentation on (originX, originY), ignoring clipping.
   Inherited classes will implement this method to effect visual rendering

   :param g: Graphics element to be drawn on
   :param origin: topLeft coordinate, the starting point for drawing inside g
   :param extent: size of the allocated drawing area, but not limited to it (no clipping)

