# GET aHEAD

## 0x1 Description

>Find the flag being held on this server to get ahead of the competition http://mercury.picoctf.net:21939/

## 0x2 Solution

On va jouer rapidement avec curl, vu le titre les informations vont se situer dans la partie HEAD de l'entête HTML:

> curl -I http://mercury.picoctf.net:21939/

retourne la réponse suivante:

>HTTP/1.1 200 OK
>flag: picoCTF{r3j3ct_th3_du4l1ty_6ef27873}
>Content-type: text/html; charset=UTF-8

Il est possible de filtrer encore plus pour avoir juste le flag qui s'affiche:

>curl -I http://mercury.picoctf.net:21939/ | grep -E -o "picoCTF{*.?}"

Le flag était donc:

>picoCTF{r3j3ct_th3_du4l1ty_6ef27873}
