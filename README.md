# Xss
XSS est l'abréviation de Cross-Site Scripting. 
Une faille XSS consiste à injecter du code directement interprétable par le navigateur Web, 
par exemple, du JavaScript ou du HTML. 
Cette attaque ne vise pas directement le site comme le ferait une injection SQL mais concerne plutôt la partie client c'est-à-dire vous (ou plutôt votre navigateur). 
Ce dernier ne fera aucune différence entre le code du site et celui injecté par le pirate, il va donc l'exécuter sans broncher. 
Les possibilités sont nombreuses : redirection vers un autre site, vol de cookies, 
modification du code HTML de la page, exécution d'exploits contre le navigateur : en bref, tout ce que ces langages de script vous permettent de faire.
Plus d'information : [Cours](https://www.hacksplaining.com/exercises/xss-stored#/)

## Rappel
Le fait d'accéder ou de se maintenir, frauduleusement, dans tout ou partie d'un système de traitement automatisé de données est puni de deux ans d'emprisonnement et de 60 000 € d'amende.
Le but est de comprendre le principe de l'attaque afin de mettre en place la sécurité adequat.

## Context Mario-no parfum
Mario-no est un site E-commerce spécialisé dans la vente de parfum. 
Une cliente a informé le service support d'une usurpation d'identitée.
Elle fait appel a votre entreprise spécialisée dans la sécurité informatique et plus spécifiquement dans les attaques présentes dans le [Top Ten de l'OWASP](https://owasp.org/Top10/).
Vous êtes le consultant qui à été choisi pour trouver la faille et produire un exemple d'attaque pour faire une démnstration au client, puis proposer mettre des protections en place pour que le problème ne se reproduise pas.

## Chercher une faille
Trouver une faille dans le site puis essayez de trouver une facon d'injecter du code malvaillant.
L'objectif: 
Vous devez récupérer les cookies du site.
Une fois la faille trouvée, renvoie les informations vers l'adresse de ton site malveilllant voir si tu les récupère bien: http://localhost/cyber/xss/hacked.php?cookie="...
Ensuite écrit un mail à ton binome et envoie lui un mail de phishing : 

Cher Client,

Nous avons le plaisir de vous informer que nous avons lancé une offre promotionnelle exclusive pour nos clients.
Pendant une durée limitée, vous pouvez bénéficier d'une réduction de 80% sur notre gamme de parfum.

Pour en profiter, il vous suffit de saisir le code promo [#PARFUMOR2024] lors de votre <a href="lienMalveillant">prochaine commande en ligne</a> ou de mentionner l'offre lors de votre prochaine visite en magasin.

N'hésitez pas à nous contacter pour plus d'informations ou pour toute demande de devis.
Nous espérons vous accueillir bientôt.

Bien à vous,

Regarder la tete de votre binome.


## Correction
Sécuriser le site en proposant mettant en place un correctif pérenne dans le temps.

