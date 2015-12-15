.. java:import:: Definition.model ResolutionAction

IBoardClickResolutionListener
=============================

.. java:package:: Definition.event
   :noindex:

.. java:type:: public interface IBoardClickResolutionListener

   An interface for the event listener for clicks on the board.

Methods
-------
resolveBoardElementClick
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method::  ResolutionAction[] resolveBoardElementClick(IGameEngine gameEngine, IBoard board, Point boardCoordinates, IPlayer player, IBoardElement clickedElement, IFigureStack clickedStack, IFigure clickedFigure)
   :outertype: IBoardClickResolutionListener

   The event that the game engine calls after every move expecting a resolution for the move. Moves that areapproved become a part of the journal.

   :param gameEngine: The gameEngine which controlls the game
   :param board: The board on which the game is played
   :param player: The player who is moving the figure
   :return:  A list of actions the game engine should do as a result of this move

