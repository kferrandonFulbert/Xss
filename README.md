# Xss
XSS est l'abréviation de Cross-Site Scripting. 
Une faille XSS consiste à injecter du code directement interprétable par le navigateur Web, 
par exemple, du JavaScript ou du HTML. 
Cette attaque ne vise pas directement le site comme le ferait une injection SQL mais concerne plutôt la partie client c'est-à-dire vous (ou plutôt votre navigateur). 
Ce dernier ne fera aucune différence entre le code du site et celui injecté par le pirate, il va donc l'exécuter sans broncher. 
Les possibilités sont nombreuses : redirection vers un autre site, vol de cookies, 
modification du code HTML de la page, exécution d'exploits contre le navigateur : en bref, tout ce que ces langages de script vous permettent de faire.

## Chercher une faille
Trouver une faille dans le site puis essayez de trouver une facon d'injecter du code malvaillant.
L'objectif: 
Vous devez récupérer les cookies du site.
