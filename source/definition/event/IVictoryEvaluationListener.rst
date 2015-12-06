.. java:import:: Definition.model ResolutionAction

IVictoryEvaluationListener
==========================

.. java:package:: Definition.event
   :noindex:

.. java:type:: public interface IVictoryEvaluationListener

   Created by hades-incarante on 10/26/2015. Interfejs za event listener za victory resolver.

Methods
-------
evaluateVictory
^^^^^^^^^^^^^^^

.. java:method::  ResolutionAction[] evaluateVictory(IGameEngine gameEngine, IBoard board, IPlayer player, ResolutionAction[] currentResolutionSet)
   :outertype: IVictoryEvaluationListener

   Event koji game engine poziva ako je prethodni resolver zahtevao proveru stanja pobede, racuna se kao deo trenutnog poteza

   :param gameEngine: gameEngine koji kontrolise igru
   :param board: instanca boarda na kojem se igra
   :param player: igrac koji pomera figuru
   :return: spisak akcija koje game engine treba da izvrsi kao posledicu ovog poteza, osnova za zurnal

