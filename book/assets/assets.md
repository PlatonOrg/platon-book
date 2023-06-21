# Assets

Les assets sont des éléments graphique avec lequel l'élèves peut interagir (exercice, activité, page, vidéo, etc...)

Les assets sont des instanciations des ressources. 

Une fois la ressource instanciée et donc publié, la ressource assets est non mutable (il faut recharger une nouvelle version pour modifier la ressouce ce qui peut avoir des conséquences sur ce que les différents élèves voient).
Les nouvelles versions de la ressource n'affecte pas les assets précédemment publié.
C'est pourquoi on appel la ressouce dans un asset une "frozen-ressource".



{% hint style="warning" %}
En cas de problème dans la version publié il est possible de **reload** l'asset. 
Cet intervention est uniquement réalisable par les enseignants en charge de l'asset ou un administrateur.
{% endhint %}

## Propriétés sur les assets

Les assets possèdent des propriétés supplémentaires aux ressources relatives à l’interaction de l'assets avec les élèves et les professeurs.

1) Les assets sont navigables : exemple un cours il est possible d'afficher le cours et les assets qu'il contient.
2) La navigation dépend de l'utilisateur : admin/prof/prof-non-editeur/élève et la navigation permet de "naviger" sur les assets
  a) Visibilité: Certaines classe d'utilisateur ne voient pas l'asset (c'est comme il n'extait pas), pour les autres il est visible mais grisé (ou autre indicateur graphique).
  b) Navigabilité: Un utilisateur vois ces cours. IL peut rentre dans un cours et voire les sections du cours. Puis rentrer dans une section pour voire le contenu (peut être plier et déplier la section). Pour montrer cela les assets sont dans une hiérachie d'objet qui sont visiblable comme une arborescence classique.
  c) Exécutable: Si l'asset est de type executable (exercice/ activité/ présentation/ etc) en fonction de l'utilisateur il est executable en mode standard (elève) ou en mode préview (autres).
  d) Parametrable :les propriétés sont manipulables par formulaire.
3) Les Tableau de bord
   Les tableau de bord d'asset permettent d'avoir des informations sur le déroulement d'un asset.
   
### Les propriétés 
  * Référence de la ressource
  * Ensemble d'utilisateur / groupes
  * Parent
  * Date d'ouverture / fermeture
  * Visibilité
  * Etiquettes
  * TODO

## Hiérarchie des assets

{% hint style="info" %}
cours <- section <- activités 
les sections sont des activités (on peut boucler sur les sections mais pas trop longtemps ;)

{% endhint %}

## Modélisation UML

{% hint style="info" %}
[https://www.plantuml.com/plantuml/dpng/NO_12i8m38RlUOhGep3KDzWOx20xJM_Y8NHn56ehJNPnxDqjTeZOIyd_9U5BBKf9vuU7rfC8DYAik41-AsnPb-ABmy0YSKwM5pXhSc72RpBmdHC7omWdYQ5px4SSIGcaTAfJpt2XwNf3fKbWnMstQQpb_BSnQ8eUUoTgaB98s-FoaIXAkwf2SpJ_Ch_qiCyypvMir8KyAN5GWmL0pM7C9xy1](lien)
{% endhint %}



