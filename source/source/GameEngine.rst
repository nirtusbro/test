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

   Created by hades-incarnate on 10/30/2015. Prva generic verzija

Constructors
------------
GameEngine
^^^^^^^^^^

.. java:constructor:: public GameEngine(JPanel playArea)
   :outertype: GameEngine

   Konstruktor

   :param playArea: panel na kome se nalazi igra i svi njeni elementi (figure, board, karte... )

Methods
-------
addBoardClickResolutionListener
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void addBoardClickResolutionListener(IBoardClickResolutionListener boardClickResolutionListener)
   :outertype: GameEngine

   Metod za dodavanje listenera koji reaguje na klik misem na board

   :param boardClickResolutionListener: listener koji se dodaje

addMoveResolutionListener
^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void addMoveResolutionListener(IMoveResolutionListener moveResolutionListener)
   :outertype: GameEngine

   Metod za dodavanje listenera koji reaguje na pomeranje figure na tabli

   :param moveResolutionListener: listener koji se dodaje

addPlayer
^^^^^^^^^

.. java:method:: @Override public IPlayer addPlayer(IPlayer playerDef)
   :outertype: GameEngine

   Metod odavanje novog igraca

   :param playerDef: igrac koji se dodaje
   :return: dodat igrac

addVictoryEvaluationListener
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void addVictoryEvaluationListener(IVictoryEvaluationListener victoryEvaluationListener)
   :outertype: GameEngine

   Metod za dodavanje listenera koji se izvrasava na kraju svakog poteza i proverava da li ima pobednika u igri

   :param victoryEvaluationListener: listener koji se dodaje

getBoard
^^^^^^^^

.. java:method:: public IBoard getBoard()
   :outertype: GameEngine

getPlayers
^^^^^^^^^^

.. java:method:: public ArrayList<IPlayer> getPlayers()
   :outertype: GameEngine

   Potrebno videti sa miljanom

removePlayer
^^^^^^^^^^^^

.. java:method:: @Override public void removePlayer(IPlayer player)
   :outertype: GameEngine

   Metod za uklanjanje igraca

   :param player: igrac koji se uklanja

restartGame
^^^^^^^^^^^

.. java:method:: @Override public void restartGame() throws OperationNotSupportedException
   :outertype: GameEngine

   Metod za ponovno pokretanje igre, posle zavrsetka prosle

setupGame
^^^^^^^^^

.. java:method:: @Override public void setupGame(IGameDefinition gameDef)
   :outertype: GameEngine

   Postavljanje igre

   :param gameDef: definicija igre koju kreira korisnik

startGame
^^^^^^^^^

.. java:method:: @Override @SuppressWarnings public void startGame()
   :outertype: GameEngine

   Metod za pocetak igrica, zapocinje se render cycle //dodace se jos

