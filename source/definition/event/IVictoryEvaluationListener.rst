.. java:import:: Definition.model ResolutionAction

IVictoryEvaluationListener
==========================

.. java:package:: Definition.event
   :noindex:

.. java:type:: public interface IVictoryEvaluationListener

   An interface for the event listener for the victory resolver.

Methods
-------
evaluateVictory
^^^^^^^^^^^^^^^

.. java:method::  ResolutionAction[] evaluateVictory(IGameEngine gameEngine, IBoard board, IPlayer player, ResolutionAction[] currentResolutionSet)
   :outertype: IVictoryEvaluationListener

   The event that the game engine calls if the previous resolver required checking if there is a winner, counts as part of the current move

   :param gameEngine: The gameEngine which controlls the game
   :param board: The board on which the game is played
   :param player: The player who is moving the figure
   :return: A list of actions the game engine should do as a result of this move

