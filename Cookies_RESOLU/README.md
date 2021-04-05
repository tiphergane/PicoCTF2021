# Cookies

## 0x1 Description

>Who doesn't love cookies? Try to figure out the best one. http://mercury.picoctf.net:17781/

## 0x2 Analyse

Encore une fois, la description est très explicite, nous allons devoir jouer avec les cookies et il y en aura surement un meilleur que les autres

Après avoir entré le nom du premier biscuit qu'ils nous propose, nous avons la structure du cookie qui nous est donnée:

![Cookie's structure](./IMG/cookie.png)

Pas besoin d'être un génie pour comprendre qu'il va falloir incrémenter la valeur contenue dans **name**

## 0x3 Résolution avec cURL

Le principe est de faire une petite boucle qui va incrémenter la valeur et appeler la vérification avec cette donnée.

Ce qui donne après quelques itérations le résultat suivant:

>curl --cookie "name=18" http://mercury.picoctf.net:17781/check
>
>flag = picoCTF{3v3ry1_l0v3s_c00k135_bb3b3535}

## 0x4 Vérification avec Cookie Quick Manager

Avec n'importe quel éditeur de cookie, vous pouvez le modifier et une fois la page rechargée voir apparaitre la solution:

![flag](./IMG/flag.png)
