ResolutionAction
================

.. java:package:: Definition.model
   :noindex:

.. java:type:: public class ResolutionAction

   Created by hades-incarnate on 10/27/2015. Objekat koji sadrzi jednu akciju koju game engine treba da izvrsi

Methods
-------
create
^^^^^^

.. java:method:: public static ResolutionAction create(ActionEnum action)
   :outertype: ResolutionAction

evaluateVictory
^^^^^^^^^^^^^^^

.. java:method:: public ResolutionAction evaluateVictory()
   :outertype: ResolutionAction

forPlayer
^^^^^^^^^

.. java:method:: public ResolutionAction forPlayer(IPlayer player)
   :outertype: ResolutionAction

getAction
^^^^^^^^^

.. java:method:: public ActionEnum getAction()
   :outertype: ResolutionAction

getTargetFigure
^^^^^^^^^^^^^^^

.. java:method:: public IFigure getTargetFigure()
   :outertype: ResolutionAction

getTargetPlayer
^^^^^^^^^^^^^^^

.. java:method:: public IPlayer getTargetPlayer()
   :outertype: ResolutionAction

getTargetStack
^^^^^^^^^^^^^^

.. java:method:: public IFigureStack getTargetStack()
   :outertype: ResolutionAction

isAnimationSuspended
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public boolean isAnimationSuspended()
   :outertype: ResolutionAction

isEvaluateVictory
^^^^^^^^^^^^^^^^^

.. java:method:: public boolean isEvaluateVictory()
   :outertype: ResolutionAction

isKeepPlayerActive
^^^^^^^^^^^^^^^^^^

.. java:method:: public boolean isKeepPlayerActive()
   :outertype: ResolutionAction

keepPlayerActive
^^^^^^^^^^^^^^^^

.. java:method:: public ResolutionAction keepPlayerActive()
   :outertype: ResolutionAction

suspendAnimation
^^^^^^^^^^^^^^^^

.. java:method:: public ResolutionAction suspendAnimation()
   :outertype: ResolutionAction

toStack
^^^^^^^

.. java:method:: public ResolutionAction toStack(IFigureStack stack)
   :outertype: ResolutionAction

usingFigure
^^^^^^^^^^^

.. java:method:: public ResolutionAction usingFigure(IFigure figure)
   :outertype: ResolutionAction

