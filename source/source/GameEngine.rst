.. java:import:: Source.generic GenericBoard

.. java:import:: sun.reflect.generics.reflectiveObjects NotImplementedException

.. java:import:: javax.naming OperationNotSupportedException

.. java:import:: java.awt.image BufferedImage

.. java:import:: java.util ArrayList

GameEngine
==========

.. java:package:: Source
   :noindex:

.. java:type:: public final class GameEngine implements IGameEngine


Constructors
------------
GameEngine
^^^^^^^^^^

.. java:constructor:: public GameEngine(JPanel playArea)
   :outertype: GameEngine

   :param playArea: The panel which contains the game and all its elements

Methods
-------
addBoardClickResolutionListener
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void addBoardClickResolutionListener(IBoardClickResolutionListener boardClickResolutionListener)
   :outertype: GameEngine

   Adds a listener that reacts to mouse clicks on the board

   :param boardClickResolutionListener: The listener to be added

addMoveResolutionListener
^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void addMoveResolutionListener(IMoveResolutionListener moveResolutionListener)
   :outertype: GameEngine

   Adds a listener that reacts to figure moves on the board

   :param moveResolutionListener: The listener to be added

addPlayer
^^^^^^^^^

.. java:method:: @Override public IPlayer addPlayer(IPlayer playerDef)
   :outertype: GameEngine

   Adds a new player during the game

   :param playerDef: The player to be added
   :return: The added player

addVictoryEvaluationListener
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void addVictoryEvaluationListener(IVictoryEvaluationListener victoryEvaluationListener)
   :outertype: GameEngine

   Adds a listener which is called by the API user and checks whether there is a winner in the game. To be called only if one of the previous resolvers requires it, in which case all the moves prior to this one are applied to the game, so that this event could determine the winner based on the move played. This event isn't mandatory, any resolver can return ActionEnum.DeclareVictory.

   :param victoryEvaluationListener: Listener to be added

getBoard
^^^^^^^^

.. java:method:: public IBoard getBoard()
   :outertype: GameEngine

   Returns the currently selected element

   :return: The selected element, null if nonexistent

getPlayers
^^^^^^^^^^

.. java:method:: public ArrayList<IPlayer> getPlayers()
   :outertype: GameEngine

   Returns all players

   :return: A list of all players

removePlayer
^^^^^^^^^^^^

.. java:method:: @Override public void removePlayer(IPlayer player)
   :outertype: GameEngine

   Removes the specified player

   :param player: The player to be removed

restartGame
^^^^^^^^^^^

.. java:method:: @Override public void restartGame() throws OperationNotSupportedException
   :outertype: GameEngine

   Restarts the game, after the last one is finished

setupGame
^^^^^^^^^

.. java:method:: @Override public void setupGame(IGameDefinition gameDef)
   :outertype: GameEngine

Declares a setup for the game, must be called before the beggining of the game.

   :param gameDef: The definition of the game

   **See also:** :java:ref:`IGameDefinition`

startGame
^^^^^^^^^

.. java:method:: @Override @SuppressWarnings public void startGame()
   :outertype: GameEngine

   Start the game. To be called after the game is defined completely. Starts the render cycle.

