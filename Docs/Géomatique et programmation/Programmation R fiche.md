# Introduction à R

Il existe 3 grands types de formations : 

* booléens
* nombre 
* chaîne de caractère

## Nombres


```
5
5*3+1
a <- 5*3+1
```

## Booléens

```
a <- TRUE   
a==2
a<2
a>=16
```
## Chaîne de caractère

```
a <- "R"
```
## Vecteurs
```
a <- c(3,5,3,6,8) 
E <- c(7,9,45,85,14,8:36,a,78)
E[] #extraire les informations d'un vecteur
E[1] #renvoie la première valeur
length(E) #donne la longueur d'un vecteur
ls() #liste les objets en mémoire
rm(a) #supprimer l'objet a
rm(list = ls()) #efface tous les objets en mémoire
```

Exercice : créer un objet x contenant successivement les valeurs
de 1 à 10, puis les valeurs 3, 4 et 5

```
x <- c(1:10,3,4,5)
```

Exercice: extraire de la 2ème à la 6ème valeur de x, puis les 9è,
11è valeurs. Stocker le résultat dans un objet X. Extraire ensuite
seulement la dernière valeur de x (juste en l'affichant, i.e. sans en
faire un objet)

```
X <- x[c(2:6,9,11)]
x[13] ou x[length(x)]
```

# Objets sous R

## Les valeurs arithmétiques

```
xlog <- log(x)
xlog10 <- log(x,base=10)
xlog==xlog10 #vérifier une condition d'égalité
xlog > xlog10
xlog <= xlog10
```

Exercice: faire la somme des valeurs n°4 à 8 de x et de l'avant dernière
valeur de x

```
sum(x[4:8],x[length(x)-1])
sum(x[c(4:8, length(x)-1)])
```

Exercice: multiplier la 2eme valeur de x par la 3eme valeur de y <-
1:4

```
y <- 1:4
x[2]*y[3]
```
Exercice: mettre à 0 à toutes les valeurs de x inférieures ou égales à
5

```
toto <- x[x>=5] #on extrait les valeurs de x >=5
x[x<=5] <- 0
```
## La fonction which()

La fonction which() donne les indices (les positions dans l'objet) des
valeurs vérifiant le critère qu'on spécifie dans la fonction

```
which(x!=0) #position des objets différents de 0
```
## La fonction seq() 

```
seq(1,10,by=2)  
seq(1,10,length.out = 5) # on veut 5 éléments entre le 5 et le 10
diff(seq(1,10,length.out = 5))
```
Exercice: pour une valeur sur 5 de l'objet x, ajouter 0.5 et prendre le
log10 de la valeur obtenue x+0.5 (les valeurs de x seront modifiées)

```
log10(x[seq(1,length(x),by=5)]+0.5)
```
Exercice: créer un objet X ne contenant qu'une valeur sur 2 de x

```
X <- x[seq(1,length(x),by = 2)]
```
## Générer des valeurs aléatoires

```
y <- rnorm(10) # génère 10 valeur aléatoire dans un loi centré réduite tourne autour de 0
mean(y)
sd(y)
```
Exercice: où sont les valeurs négatives de y ?

```
which(y<0)
```
## Matrices

```
A0 <- matrix(data = rnorm(25),nrow=5,ncol=5) # matrice de 5 lignes par 5 colonnes
dim(A0)
A0[1,1] # élément de la première ligne de la première colonne
A <- matrix(data = NA,nrow=4,ncol=4)
```
Exercice: dans la matrice A, extraire 1 valeur sur 2 de la colonne 3, la
3eme valeur de la colonne 2, toute la colonne 1,les 1ere et 3e valeurs
de la colonne 4.

```
A[1,] <- 0
A[2,] <- rnorm(4)
A[3,] <- seq(4,56, length.out = 4)
A[4,c(1,4)] <- 0
A[4,c(2,3)] <- c(4,5)
```
Ranger toutes ces valeurs dans un objet a de type
vecteur les unes à la suite des autres (dans l'ordre énoncé
précédemment).

```
a <- c(A[seq(from=1, to =4, by =2),3], #extraire 1 valeur sur 2 de la colonne 3,
A[3,2], #la 3eme valeur de la colonne 2, 
A[,1], #toute la colonne 1,
A[c(1,3),4]) #les 1ere et 3e valeurs de la colonne 4.
``` 

Modifier  la matrice  A  en  triant  dans  l'ordre  décroissant  les  valeurs  de  la  3e colonne de A 

```
A[,3] <- sort(A[,3], decreasing = TRUE)
```