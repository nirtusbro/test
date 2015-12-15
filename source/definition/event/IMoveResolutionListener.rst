IMoveResolutionListener
=======================

.. java:package:: Definition.event
   :noindex:

.. java:type:: public interface IMoveResolutionListener

   Created by hades-incarante on 10/26/2015. INterfejs za event listener za glavni game resolver.
   An interface for the event listener for clicks on the board.

Methods
-------
resolveMove
^^^^^^^^^^^

.. java:method::  ResolutionAction[] resolveMove(IGameEngine gameEngine, IBoard board, IPlayer player, IBoardElement sourceElement, IBoardElement destinationElement, IFigureStack sourceStack, IFigureStack destinationStack, IFigure figureMoving)
   :outertype: IMoveResolutionListener

   Event koji game engine poziva posle svakog poteza, ocekujuci razresenje poteza. Potezi koji se dozvole postaju deo zurnala.

   :param gameEngine: The gameEngine which controlls the game
   :param board: The board on which the game is played
   :param player: The player who is moving the figure
   :param sourceElement: The source board element from which the move is being played
   :param destinationElement: The target board element from which the move is being played
   :param sourceStack: The source stack from which the move is being played
   :param destinationStack: The target stack from which the move is being played
   :param figureMoving: The figure which is being moved
   :return: A list of actions the game engine should do as a result of this move

