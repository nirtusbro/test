.. java:import:: javax.naming OperationNotSupportedException

IGameEngine
===========

.. java:package:: Definition
   :noindex:

.. java:type:: public interface IGameEngine

   Created by hades-incarnate on 10/20/2015.

Methods
-------
addBoardClickResolutionListener
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method::  void addBoardClickResolutionListener(IBoardClickResolutionListener boardClickResolutionListener)
   :outertype: IGameEngine

   Metod za dodavanje listenera koji reaguje na klik misem na board

   :param boardClickResolutionListener: Listener koji se dodaje

addMoveResolutionListener
^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method::  void addMoveResolutionListener(IMoveResolutionListener moveResolutionListener)
   :outertype: IGameEngine

   Metod za dodavanje listenera koji reaguje na pomeranje figure na tabli

   :param moveResolutionListener: Listener koji se dodaje

addPlayer
^^^^^^^^^

.. java:method::  IPlayer addPlayer(IPlayer playerDef)
   :outertype: IGameEngine

   Metod odavanje novog igraca u toku igre

   :param playerDef: igrac koji se dodaje
   :return: dodat igrac

addVictoryEvaluationListener
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method::  void addVictoryEvaluationListener(IVictoryEvaluationListener victoryEvaluationListener)
   :outertype: IGameEngine

   Metod za dodavanje listenera koji se izvrasava na zahtev API korisnika i proverava da li ima pobednika u igri. Poziva se samo ako neki od prethodnih resolvera to zahteva u kom slucaju se na igru primenjuju sve zahtevane akcije do ove, da bi ovaj event mogao da analizira pobedu na osnovu odigranog poteza. NOTE: Ovaj event nije obavezan, bilo koji od rosolvera moze da vrati ActionEnum.DeclareVictory !

   :param victoryEvaluationListener: Listener koji se dodaje

removePlayer
^^^^^^^^^^^^

.. java:method::  void removePlayer(IPlayer player)
   :outertype: IGameEngine

   Metod za uklanjanje igraca

   :param player: Igrac koji se uklanja

restartGame
^^^^^^^^^^^

.. java:method::  void restartGame() throws OperationNotSupportedException
   :outertype: IGameEngine

   Metod za ponovno pokretanje igre, posle zavrsetka prosle

setupGame
^^^^^^^^^

.. java:method::  void setupGame(IGameDefinition gameDef)
   :outertype: IGameEngine

   Pre pocetka igre, mora da se deklarise setup, to se radi pozivanjem ove metode.

   :param gameDef: definicija igre

   **See also:** :java:ref:`IGameDefinition`

startGame
^^^^^^^^^

.. java:method::  void startGame()
   :outertype: IGameEngine

   Nakon sto je igra potpuno definisana, ovde pocinje izvodjenje igre. Ovo i zapocinje render cycle

