# Dopé votre function Math en javascript et prototypé plus rapidement

La fonction ‘Math’ en JavaScript se retrouve plus limitée que les possibilités de son coussin le *Processing*. C’est pourquoi ce script ajoute directement à la fonction ‘Math’ des fonctions de calcul courant et bien utile pour le prototypage ou le dessin génératif.

## Ajouter le script
	<script src="http://link.victorien.net/math.js" ></script>	

## Le random
La fonction initiale ‘Math.random()’ retourne exclusivement un chiffre compris entre 0 et 1. Voici quelques ajouts supplémentaires :
	
	//Retourne un chiffre aléatoire compris entre 0 et a.
	Math.random(a)
	
	//Retourne un chiffre aléatoire compris entre a et b.
	Math.random(a,b)
	
	//Retourne une valeur piochée aléatoirement dans le tableau.
	Math.random(array)
	

## La distance et direction
Calculer l’angle, la distance entre deux points ou encore le coefficient directeur :
	
	//Cacule la distance entre les deux points.
	Math.distance(x1, y1, x2, y2)
	
	//Calcule le coefficient directeur entre ces deux points.
	Math.direction(x1, x2)
	
	//Cacule l’angle en Radian entre ces deux points.
	Math.angle(x1, y1, x2, y2)
	
	//Convertis une valeur initialement en radian en degré
	Math.radToDegree()
	
	//Convertis une valeur initialement en degré en radian.
	Math.degreeToRad()
	

## Cordonné polaire

Caculer la position d’un point en fonction de ses coordonnées polaires peut se révéler pratique.

Initialement le point d’origine se trouve en (0,0) soit dans le coin supérieur gauche de l’écran. Si vous souhaitez modifier la position du point d’origine pour les coordonnées polaire, vous pouvez le faire grâce à cette fonction :

	Math.radial.changeOrigin(x, y)


Il est aussi possible de convertis des coordonnées polaires (angle, rayon) en coordonnées cartésiennes (x, y) ou l'inverse
	
	//coordonnées polaire vers coordonnées cartésiennes
	//retourne un objet du type {r:number, a:number}
	Math.radial.toXY(rayon, angle)
	
	//coordonnées cartésiennes vers coordonnées polaire
	//retourne un objet du type {x:number, y:number}
	Math.radial.toPolar(x,y)
	
	
