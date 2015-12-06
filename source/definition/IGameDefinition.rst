.. java:import:: java.awt.image BufferedImage

.. java:import:: java.util List

IGameDefinition
===============

.. java:package:: Definition
   :noindex:

.. java:type:: public interface IGameDefinition

   Created by hades-incarnate on 10/20/2015. Ovaj interfejse se ne implementira u API-u, njega implementira kreator igrice i instancu prosledjuje u game-engine

Methods
-------
getBackground
^^^^^^^^^^^^^

.. java:method::  BufferedImage getBackground()
   :outertype: IGameDefinition

   Slika koja ce biti pozadina board igrice

   :return: Ucitana slika

getBoard
^^^^^^^^

.. java:method::  IBoard getBoard()
   :outertype: IGameDefinition

   Deklaracije boarda na kojem se igra

   :return: Board

getPlayers
^^^^^^^^^^

.. java:method::  List<IPlayer> getPlayers()
   :outertype: IGameDefinition

   Inicijalna formacija igraca koji zapocinju igru

   :return: Niz igraca

