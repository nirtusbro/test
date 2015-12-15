.. java:import:: javax.naming OperationNotSupportedException

IGameEngine
===========

.. java:package:: Definition
   :noindex:

.. java:type:: public interface IGameEngine

   

Methods
-------
addBoardClickResolutionListener
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method::  void addBoardClickResolutionListener(IBoardClickResolutionListener boardClickResolutionListener)
   :outertype: IGameEngine

   Adds a listener that reacts to mouse clicks on the board

   :param boardClickResolutionListener: The listener to be added

addMoveResolutionListener
^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method::  void addMoveResolutionListener(IMoveResolutionListener moveResolutionListener)
   :outertype: IGameEngine

   Adds a listener that reacts to figure moves on the board

   :param moveResolutionListener: The listener to be added

addPlayer
^^^^^^^^^

.. java:method::  IPlayer addPlayer(IPlayer playerDef)
   :outertype: IGameEngine

   Adds a new player during the game

   :param playerDef: The player to be added
   :return: The added player

addVictoryEvaluationListener
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method::  void addVictoryEvaluationListener(IVictoryEvaluationListener victoryEvaluationListener)
   :outertype: IGameEngine

   Adds a listener which is called by the API user and checks whether there is a winner in the game. To be called only if one of the previous resolvers requires it, in which case all the moves prior to this one are applied to the game, so that this event could determine the winner based on the move played. This event isn't mandatory, any resolver can return ActionEnum.DeclareVictory.

   :param victoryEvaluationListener: Listener to be added

removePlayer
^^^^^^^^^^^^

.. java:method::  void removePlayer(IPlayer player)
   :outertype: IGameEngine

   Removes the specified player

   :param player: The player to be removed

restartGame
^^^^^^^^^^^

.. java:method::  void restartGame() throws OperationNotSupportedException
   :outertype: IGameEngine

   Restarts the game, after the last one is finished

setupGame
^^^^^^^^^

.. java:method::  void setupGame(IGameDefinition gameDef)
   :outertype: IGameEngine

   Declares a setup for the game, must be called before the beggining of the game.

   :param gameDef: The definition of the game

   **See also:** :java:ref:`IGameDefinition`

startGame
^^^^^^^^^

.. java:method::  void startGame()
   :outertype: IGameEngine

   Start the game. To be called after the game is defined completely. Starts the render cycle.

