# Chromatographie

La chromatographie est une méthode séparative dans le but de séparer les composés et de les doser.

On va utiliser la chromatographie pour analyser les mélanges, chromatographie **semi-préparative ou préparative** afin de récupérer les produits purs.

On l'utilise aussi pour l'identification des éléments par couplage.

On va donc séparer les molécules d'un mélange.

Il existe plusieurs techniques chromatographique : 

* selon la nature de la phase mobile
	* en phase gazeuse
    * en phase supercritique
    * en phase liquide
    
Partage des constituants (solutés) des mélanges entre deux phases :

* phase stationnaire (PS) : elle ne bouge pas
* phase mobile (PM) : elle bouge

![Principe](Images/22.jpg)

A partir du détecteur nous aurons un chromatograme avec un pique par molécule.

Chromatographie en phase liquide

* sur colonne : contenue dans un tube
* de surface: contenue sur une surface (CCM)

Interaction entre solutés et phase stationnaire :

* ionique
* exclusion
* adsorption
* partage

![Classification des méthodes chromatographiques](Images/32.jpg)

Chromatographie d'exclusion : phase polimère, séparation en fonction de la taille des molécules

Chromatographie ionique : phase stationnaire chargée, séparation entre les interactions ioniques

![Phénomènes chromatographiques](Images/42.jpg)

Chromatographie liquide et chromatographie gazeuse

* chromatographie de partage, interactions de van der waals et de liaisons H, on va utilisé le silice
* chromatographie d'adsorption (propriétés de surface), interactions en surface (par exemple charbon actif dans les hôtes). Il est beaucoup moins utilisé

Phénomènes chromatographiques :

* partage du soluté entre les 2 phases : soluté phase mobile retenue par la phase stationnaire, paratge de façon équilibré. Réalisé par un constante d'équilibre : fonction de la température **lnK = delta G°/RT**. Plus les molécules sont fortes, plus le soluté va être retenu en phase stationnaire; **grandeurs thermodynamique**

* dispersion des molécules au cours de leur transfert dans la colonne : déplacement de phase mobile; **grandeurs cinétique**

* combinaison des 2 processus : résolution

Aire du pic pour remonter à la concentration du soluté.

Grandeurs fondamentales : on va utiliser des mélanges de solvant. 

![Coefficient de partage](Images/51.jpg)

## Grandeurs thermodynamiques :

### Facteur de rétention

** facteur de rétention**, k : lié au coefficient de partage, quantité de soluté dans la phase stationnaire sur la phase mobile.

k : Qs/Qm = CsVs / CmVm = K * Vs/Vm (constante pour un système chromatographique donné)

Si on augmente k il faut diminuer la température

**k = (tr - tm)/tm** (sans unité)

tr = temps de rétention : pic  et tm = temps de molécule pas retenue par le solvant

k dépend : 

* de la nature des phases (PS et PM).
* de la température

k  est dépendant :

* du débit de la PM
* des dimensions géométriques de la colonne

### La sélectivité

**La sélectivité** est temps entre 2 pics consécutives : distance entre les 2 pics : montre une différence d'interaction. Si un seul pic : co-élution des deux composés

![La sélectivité](Images/62.jpg)

alpha dépend :

* de la température
* du système de phases, dépend de la phase mobile et de la phase stationnaire

Phénomènes de dispersion en chromatographie, les molécules ne vont pas arriver toutes en même temps. Elle va être fonction de la vitesse de la phase mobile -> grandeurs cinétiques :

* N : nombre de plateaux théorique
* HEPT : hauteur équivalente à un plateau théorique 

Elles vont être indépendantes de la températures mais dépendant en fonction de la phase mobile.

![Phénomènes de diffusion en chromatographie](Images/71.jpg)

Importance de l'efficacité d'une colonne chromatographique : plus la vauler de N est grand, plus le pic sera fin. Cette diffusion est dû là la dispersion des solutés. Cette diffusion est "mesurée" par l'efficacité de la colonne chromatographique.

## Grandeurs cinétiques

Plus le nombre d'équilibre est grand, plus le système sera efficace.

La théorie des plateaux établit que, après un certain parcours dans la colonne, les pics d'élution peuvent être assimilés à des courbes de Gauss.

![Efficacité d'une colonne chromatographique](Images/82.jpg)

Nth est un nombre entier et n'a pas d'unité. Elle va être dépendante de la vitesse de la phase mobile.

## Résolution

La résolution est deux fois la différence du temps de rétention sur la somme des largeur de pic à la base. Il existe une valeur seuil qui montre que c'est correcte : 1,5. Valeur minimale de résolution à avoir.

![Résolution](Images/92.jpg)

Pour augmenter R on augmente la distance entre les deux pics, **la sélectivité** et il faut diminuer les largeurs de pics, augmenter **l'efficacité** du système.

Il faut d'abord optimiser alpha en l'augmentant puis N en l'augmentant (pic plus fin) et enfin k mais il augmente la durée globale de l'analyse.

k = 0, pas de rétention donc le soluté n'est pas du tout fixé sur le système.

mélange simple : moins de 5 composés et mélange complexe entre 2 et 10 composés

![Exemple](Images/111.jpg)

# Chromatographie liquide haute performance HPLC

![Système HPLC](Images/121.jpg)

![Exemple](Images/122.jpg)

* PM : mélange de solvant, le solvant de base est l'eau
* boucle d'injection 
* colonne
* détecteur : détection UV
* traitement et acquisition du signal 

On va séparer les espèces d'un mélange partage entre une phase mobile est une phase stationnaire. Chaque soluté injecté sur la colonne est soumis à deux effets antagonistes : un effet d'entraînement par la phase mobile dans laquelle il est soluble et un effet de rétention par la phase stationnaire avec l'aquelle il interagit. Le soluté doit être soluble.

![Définition du système HPLC](Images/132.jpg)

## Chromatographie de partage

La séparation des différences de solubilité des solutés dans la phase mobile et des différentes interactions des solutés avec les groupements organiques greffées sur la phase stationnaire à base de silice.

On va utilisé la chromatographie de partage à polarité de phases inverses : le solvant de base est l'eau avec un solvant organique et la phase stationnaire et la silice dans lequel ont à formé  un modèle organique. La phase stationnaire sera moins polaire que la phase mobile.

La silice est très polaire donc absorbante. La surface sont des silanols (groupement réactif) qui sont polaires afin d'avoir les interactions. Sur ces groupements en phase inverse on mettra des longues chaines hydrocarboné octadecyle. On utilise pas seulement la silice car l'eau s'accroche à celle -ci. On utilisera une colonne C18.

## Les grandeurs thermodynamiques

Les facteurs essentiels modifiant la sélectivité alpha sont : 

* la phase stationnaire
	* nature du greffon
    * nature de la silice

* la phase mobile : force éluante
	* nature du solvant organique
    * composition eau - solvant dynamique (il faut qu'il soit missible avec l'eau)

* (la température) : colonne à température ambiente, on ne peut pas la modifier.

Composition de la phase mobile

![Composition du solvant](Images/161.jpg)
