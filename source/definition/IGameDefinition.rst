.. java:import:: java.awt.image BufferedImage

.. java:import:: java.util List

IGameDefinition
===============

.. java:package:: Definition
   :noindex:

.. java:type:: public interface IGameDefinition

   

Methods
-------
getBackground
^^^^^^^^^^^^^

.. java:method::  BufferedImage getBackground()
   :outertype: IGameDefinition

   Sets the image which will be the game's background

   :return: The background image

getBoard
^^^^^^^^

.. java:method::  IBoard getBoard()
   :outertype: IGameDefinition

   Declaration of the board on which the game will be played

   :return: The board

getPlayers
^^^^^^^^^^

.. java:method::  List<IPlayer> getPlayers()
   :outertype: IGameDefinition

   The initial formation of all the players that will start the game

   :return: A list of players

