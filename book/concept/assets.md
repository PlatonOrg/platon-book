---
description: Definition du concept d'asset
---

# Assets

Les assets sont des éléments graphique avec lequel l'élèves peut interagir (exercice, activité, page, vidéo, etc...)

Les assets sont des instanciations des ressources.

Une fois la ressource instanciée et donc publié, la ressource assets est non mutable (il faut recharger une nouvelle version pour modifier la ressouce ce qui peut avoir des conséquences sur ce que les différents élèves voient). Les nouvelles versions de la ressource n'affecte pas les assets précédemment publié. C'est pourquoi on appel la ressource dans un assets une "frozen-ressource".

{% hint style="warning" %}
En cas de problème dans la version publié il est possible de **reload** l'asset. Cet intervention est uniquement réalisable par les enseignants en charge de l'asset ou un administrateur.
{% endhint %}

## Propriétés sur les assets

Les assets possèdent des propriétés supplémentaires aux ressources relatives à l’interaction de l'assets avec les élèves et les professeurs.

1. Les assets sont navigables : exemple un cours il est possible d'afficher le cours et les assets qu'il contient.
2.  La navigation dépend de l'utilisateur : admin/prof/prof-non-editeur/élève et la navigation permet de "naviger" sur les assets:

    A) Visibilité: Certaines classe d'utilisateur ne voient pas l'asset (c'est comme il n'extait pas), pour les autres il est visible mais grisé (ou autre indicateur graphique).&#x20;

    B) Navigabilité: Un utilisateur vois ces cours. IL peut rentre dans un cours et voire les sections du cours. Puis rentrer dans une section pour voire le contenu (peut être plier et déplier la section). Pour montrer cela les assets sont dans une hiérachie d'objet qui sont visiblable comme une arborescence classique.&#x20;

    C) Exécutable: Si l'asset est de type executable (exercice/ activité/ présentation/ etc) en fonction de l'utilisateur il est executable en mode standard (elève) ou en mode préview (autres). d) Parametrable :les propriétés sont manipulables par formulaire.
3. Les Tableau de bord Les tableau de bord d'asset permettent d'avoir des informations sur le déroulement d'un asset.

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
cours <- section <- activités les sections sont des activités (on peut boucler sur les sections mais pas trop longtemps ;)
{% endhint %}

## Modélisation UML

<figure><img src="https://www.plantuml.com/plantuml/png/NP2nJWCn44Jx_OgHIwG8-8E4WnGeLHBH80fpDpaiEJRoxb5mohzZuWWGbULvzjFiBjLyiUaOfOjU5IjL6cQHkvmZdeA6rqZ07NA1lH5gqy1awcGVZhptHko-3N1v-c0r5JhyieSqYCX9BlProPzCMwhcgVISPMSbf14_oPO75gQUa4VDQHqO1mpUl6XxQS4YPU_7vnUO7rLEkBZTgkzPpoudApbY4zGSl6BLRJ2VIxJXhXOBk5ltlynVUdDTUVtNidPlvDqNfkez0rao3NLtNm00" alt="" width="563"><figcaption></figcaption></figure>
