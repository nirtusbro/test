.. java:import:: Definition IFigure

.. java:import:: Definition IPlayer

.. java:import:: java.util ArrayList

Player
======

.. java:package:: Source
   :noindex:

.. java:type:: public class Player extends MetadataContainer implements IPlayer

   Created by hades-incarnate on 10/30/2015. generic player

Constructors
------------
Player
^^^^^^

.. java:constructor:: public Player(String name)
   :outertype: Player

   Konstruktor

   :param name: Inicijalizacija imena

Methods
-------
addFigure
^^^^^^^^^

.. java:method:: public void addFigure(IFigure figure)
   :outertype: Player

   Dodavanje figure

   :param figure: Zadata figura

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: Player

   Vraca ime igraca

   :return: Ime igraca

removeFigure
^^^^^^^^^^^^

.. java:method:: public void removeFigure(IFigure figure)
   :outertype: Player

   Uklanjanje figure

   :param figure: Zadata figura

setName
^^^^^^^

.. java:method:: @Override public void setName(String value)
   :outertype: Player

   Postavlja ime igraca

   :param value: Zadato ime

