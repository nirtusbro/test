.. java:import:: Definition IVisualPresentation

.. java:import:: java.util List

CompositeVisualPresenter
========================

.. java:package:: Source
   :noindex:

.. java:type:: public final class CompositeVisualPresenter extends ArrayList<IVisualPresentation> implements IVisualPresentation, List<IVisualPresentation>

   Created by hades-incarnate on 11/16/2015. More complex, composite visual presenter, encapsulating composite implementation, should be inherited by complex multi-element presentations (say bitmap on a shape inside a circle, etc)

Methods
-------
addChildPresenters
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void addChildPresenters(IVisualPresentation presenter)
   :outertype: CompositeVisualPresenter

   Add child presenter

   :param presenter: new child visual presenter

getChildPresenters
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public List<IVisualPresentation> getChildPresenters()
   :outertype: CompositeVisualPresenter

   Return all child presenters

   :return: A list of child visual presenters

removeChildPresenters
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void removeChildPresenters(IVisualPresentation presenter) throws NoSuchElementException
   :outertype: CompositeVisualPresenter

   Remove child presenter

   :param presenter: existing child presenter to remove

render
^^^^^^

.. java:method:: @Override public void render(Graphics2D g, Point origin, Point extent)
   :outertype: CompositeVisualPresenter

   Renders composite presentation on (originX, orignY), ignoring clipping, by rendering all of its children

   :param g: Graphics element on which to draw
   :param origin: topLeft coordinate from which to draw inside g
   :param extent: size of the allocated drawing area, but not limited to it (no clipping)

