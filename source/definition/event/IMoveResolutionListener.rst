IMoveResolutionListener
=======================

.. java:package:: Definition.event
   :noindex:

.. java:type:: public interface IMoveResolutionListener

   Created by hades-incarante on 10/26/2015. INterfejs za event listener za glavni game resolver.

Methods
-------
resolveMove
^^^^^^^^^^^

.. java:method::  ResolutionAction[] resolveMove(IGameEngine gameEngine, IBoard board, IPlayer player, IBoardElement sourceElement, IBoardElement destinationElement, IFigureStack sourceStack, IFigureStack destinationStack, IFigure figureMoving)
   :outertype: IMoveResolutionListener

   Event koji game engine poziva posle svakog poteza, ocekujuci razresenje poteza. Potezi koji se dozvole postaju deo zurnala.

   :param gameEngine: gameEngine koji kontrolise igru
   :param board: instanca boarda na kojem se igra
   :param player: igrac koji pomera figuru
   :param sourceElement: izvorisni board element sa kojeg se odigrava potez
   :param destinationElement: odredisni board element sa kojeg se odigrava potez
   :param sourceStack: izvorisni stack sa kojeg se odigrava potez
   :param destinationStack: odredisni stack sa kojeg se odigrava potez
   :param figureMoving: figura koja se pomera
   :return: spisak akcija koje game engine treba da izvrsi kao posledicu ovog poteza, osnova za zurnal

