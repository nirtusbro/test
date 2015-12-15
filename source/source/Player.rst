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

   :param name: Name initialization

Methods
-------
addFigure
^^^^^^^^^

.. java:method:: public void addFigure(IFigure figure)
   :outertype: Player

   Adds a figure

   :param figure: Figure to be added

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: Player

   Returns the player's name

   :return: Player name

removeFigure
^^^^^^^^^^^^

.. java:method:: public void removeFigure(IFigure figure)
   :outertype: Player

   Removes a figure

   :param figure: Figure to be removed

setName
^^^^^^^

.. java:method:: @Override public void setName(String value)
   :outertype: Player

   Sets the player's name

   :param value: Player name

