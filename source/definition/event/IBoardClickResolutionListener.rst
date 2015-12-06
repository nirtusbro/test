.. java:import:: Definition.model ResolutionAction

IBoardClickResolutionListener
=============================

.. java:package:: Definition.event
   :noindex:

.. java:type:: public interface IBoardClickResolutionListener

   Created by hades-incarante on 10/26/2015. Interfejs za event listener za kllik na tablu.

Methods
-------
resolveBoardElementClick
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method::  ResolutionAction[] resolveBoardElementClick(IGameEngine gameEngine, IBoard board, Point boardCoordinates, IPlayer player, IBoardElement clickedElement, IFigureStack clickedStack, IFigure clickedFigure)
   :outertype: IBoardClickResolutionListener

   Event koji game engine poziva posle svakog poteza, ocekujuci razresenje poteza. Potezi koji se dozvole postaju deo zurnala.

   :param gameEngine: gameEngine koji kontrolise igru
   :param board: instanca boarda na kojem se igra
   :param player: igrac koji pomera figuru
   :return: spisak akcija koje game engine treba da izvrsi kao posledicu ovog poteza, osnova za zurnal

