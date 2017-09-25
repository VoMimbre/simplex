# simplex
Implementation en python de la méthode du simplexe pour optimiser un panier d'achat 
pour alimenter un Marché A a prtir d'un Marché B
les contraintes sont 
1 le volume maximum transportable avec un plafond de 370.000m3
2 le montant de l'investissement 
3 le nombre d'items différents maximum avec un plafond de 50

Document http://www.phpsimplex.com/fr/theorie_modelisation_problemes.htm

Les étapes pour modeler un problème sont les suivants:

Etape 1: Déterminer les variables de décision et les formuler de façon algébrique.

X1,..., Xn

Etape 2: Déterminer les contraintes et les formuler comme des équations ou des inéquations dépendantes des variables de décision:

A11·X1 + A12·X2 + ... + A1n·Xn =, =, ó = b1
A21·X1 + A22·X2 + ... + A 2n·Xn =, =, ó = b2
...
Am1·X1 + Am2·X2 + ... + Amn·Xn =, =, ó = bm

Etape 3: Présenter toutes les conditions implicitement établies conformément à la nature des variables: qu'elles ne peuvent pas être négatives, qu'elles soient entières, qu'elles ne peuvent que prendre valeurs déterminées, ...

X1,..., Xn = 0
X1,..., Xn sont des numéros entiers, ou sont booléenne,...

Etape 4: Déterminer la fonction objectif.

Maximiser ou minimiser Z = C1·X1 + C2·X2 + ... + Cn·Xn

autre source https://hubpages.com/technology/Simplex-Algorithm-in-Python


Etape 1 : sur le marché A 
relever les prix de chaque produit dont il s'est vendu pour plus que MontantMini en 1 semaine 
Etape 2 : sur le marché B
relever les prix de ces même produits
Etape 3 : Calculer la marge entre les deux marchés pour chaque item, la ramener a la marge/m3
Etape 4 : Déterminer les contraintes avec les réponses et les limites
	A le volume maximum transportable avec un plafond de 370.000m3
	B le montant de l'investissement 
	C le nombre d'items différents maximum avec un plafond de 50 


