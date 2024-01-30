# simulation_presence
Automatisme qui allume de manière aléatoire des light ou des switch entre le coucher et le lever du soleil lorsque l'alarme est sur armed. Les lumières sont éteintes après le lever du soleil.

l'automatisme est actif si l'alarme est enclenchée ( armed ou armed_away ) 
l'automatisme se lance toutes les 20 minutes
l'automatisme appelle un premier script ( simul_presence ) avec une des entités choisie aléatoirement dans la liste, celui-ci active l'entité pour une durée aléatoire ( entre 10 et 50 minutes ) puis le désactive.
le mode parallele a été choisi pour permettre plusieurs scripts de cohabiter 
lorsque le soleil est levé le script eteindre_toutes_les_entites est appelé avec la liste complète des entités.
