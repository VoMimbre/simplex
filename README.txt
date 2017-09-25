# simplex
Implementation en python de la m�thode du simplexe pour optimiser un panier d'achat 
pour alimenter un March� A a prtir d'un March� B
les contraintes sont 
1 le volume maximum transportable avec un plafond de 370.000m3
2 le montant de l'investissement 
3 le nombre d'items diff�rents maximum avec un plafond de 50

Document http://www.phpsimplex.com/fr/theorie_modelisation_problemes.htm

Les �tapes pour modeler un probl�me sont les suivants:

Etape 1: D�terminer les variables de d�cision et les formuler de fa�on alg�brique.

X1,..., Xn

Etape 2: D�terminer les contraintes et les formuler comme des �quations ou des in�quations d�pendantes des variables de d�cision:

A11�X1 + A12�X2 + ... + A1n�Xn =, =, � = b1
A21�X1 + A22�X2 + ... + A 2n�Xn =, =, � = b2
...
Am1�X1 + Am2�X2 + ... + Amn�Xn =, =, � = bm

Etape 3: Pr�senter toutes les conditions implicitement �tablies conform�ment � la nature des variables: qu'elles ne peuvent pas �tre n�gatives, qu'elles soient enti�res, qu'elles ne peuvent que prendre valeurs d�termin�es, ...

X1,..., Xn = 0
X1,..., Xn sont des num�ros entiers, ou sont bool�enne,...

Etape 4: D�terminer la fonction objectif.

Maximiser ou minimiser Z = C1�X1 + C2�X2 + ... + Cn�Xn

autre source https://hubpages.com/technology/Simplex-Algorithm-in-Python


Etape 1 : sur le march� A 
relever les prix de chaque produit dont il s'est vendu pour plus que MontantMini en 1 semaine 
Etape 2 : sur le march� B
relever les prix de ces m�me produits
Etape 3 : Calculer la marge entre les deux march�s pour chaque item, la ramener a la marge/m3
Etape 4 : D�terminer les contraintes avec les r�ponses et les limites
	A le volume maximum transportable avec un plafond de 370.000m3
	B le montant de l'investissement 
	C le nombre d'items diff�rents maximum avec un plafond de 50 


