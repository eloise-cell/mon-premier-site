# 📒 Mon carnet de bord

**Nom : BOEDOT**

**Prénom : Eloïse** 

**Adresse de mon site :** https://______.pythonanywhere.com](https://elobdt.pythonanywhere.com)

> Modifiez ce fichier directement sur GitHub (icône crayon ✏️) pour répondre aux questions de chaque exercice.
> Écrivez avec vos propres mots : une réponse courte et juste vaut mieux qu'un long copier-coller ! 🙂

---

## 🟢 Exercice 1 — Mon premier déploiement

1. Où se trouve physiquement le code qui fabrique votre page : sur votre ordinateur, sur GitHub ou sur PythonAnywhere ?

   > sur GitHub

2. Pourquoi votre voisin(e) peut-il voir votre site, alors que vous n'avez rien installé sur son ordinateur ?

   > parce que mon site est sur un serveur connecté à Internet.

---

## 🟢 Exercice 2 — Les URL et les routes

1. Dans l'URL `https://www.google.com/maps`, quel est le nom de domaine ? Quel est le chemin ?

   > le nom de domaine est "www.google.com" et le chemin est "/maps"

2. Que veut dire le message *Not Found* ? Qui l'a envoyé : votre navigateur ou le serveur ?

   > Not found veut dire introuvable et c'est le serveur qui l'envoie

3. Que se passe-t-il si deux fonctions portent le même nom dans `flask_app.py` ? (Indice : essayez, puis lisez l'Error log.)

   > Cela va signaler une erreur.

---

## 🔵 Exercice 3 — Le langage HTML

1. Quelle est la différence entre ce que le serveur **envoie** et ce que le navigateur **affiche** ?

   > Le serveur envoie du code et le navigateur affiche la page web

2. À quoi servent les balises `<h1>`, `<p>`, `<ul>` et `<li>` ?

   > h1, pour le titre principal ; p, pour un paragraphe ; ul, pour des listes à puces ; li, pour dire ce que l'on met dans la liste.

3. Pourquoi l'image s'affiche-t-elle alors qu'elle n'est pas sur votre serveur ?

   > Parce que on met son URL

---

## 🔵 Exercice 4 — Les templates

1. Pourquoi est-ce une bonne idée de séparer le code Python et le HTML ? (Pensez à une équipe avec un développeur et un graphiste.)

   > Car le développeur peut se concentrer sur la partie codage pendant que le graphiste s'occupe de la partie HTML

2. Les `{{ prenom }}` sont-ils remplacés par le serveur ou par le navigateur ? Comment l'avez-vous vérifié ?

   > _Ma réponse :_ 

---

## 🔵 Exercice 5 — Le CSS et les liens

1. Quelle est la différence de rôle entre le HTML et le CSS ?

   > Le HTML décrit la structure (ceci est un titre, ceci est une liste…), tandis que le CSS décrit l'apparence (couleurs, polices, marges…). 

2. Pour afficher votre page `/presentation`, combien de fichiers le navigateur doit-il télécharger ? (Vous pourrez le vérifier à l'exercice suivant !)

   > Au moins 2

3. Pourquoi faut-il parfois faire **Ctrl + F5** pour voir les changements de CSS ?

   > Car cela permet de recharger la page pour afficher la nouvelle version

---

## 🟣 Exercice 6 — Espionner le navigateur

1. Que signifie HTTP ? Qui envoie la **requête** et qui envoie la **réponse** ?

   > HTTP = HyperText Transfer Protocol (protocole de transfert hypertexte). Le navigateur envoie la requête. Le serveur envoie la réponse.

2. Combien de requêtes votre page `/presentation` a-t-elle déclenchées ? Lesquelles ?

   > 1 requêtes, une pour l'HTML

3. Que signifie le code `200` ? Et le code `404` de la favicon ?

   > Le code 200 signifie que la requête a réussi et que le serveur a envoyé le contenu demandé. Le code 404 signifie que la ressource demandée est introuvable. Dans ce cas, le navigateur n'a pas trouvé la favicon du site.

4. Pourquoi les modifications faites dans l'onglet Éléments ne sont-elles pas visibles par les autres visiteurs ?

   > Car les modifications sont faites uniquement sur mon navigateur. Elles ne changent pas le vrai site enregistré sur le serveur. Les autres visiteurs ne les voient donc pas.

---

## 🟣 Exercice 7 — Envoyer des informations dans l'URL

1. Dans l'URL `https://www.youtube.com/results?search_query=chat`, quel est le nom du paramètre ? Quelle est sa valeur ?

   > Le nom du paramètre est search_query et sa valeur est chat.

2. Pourquoi le serveur plante-t-il avec `a=bonjour` ? Que faudrait-il faire pour l'éviter ?

   > Le serveur plante parce qu'il reçoit du texte alors qu'il attend sûrement un nombre. Il faudrait vérifier les informations reçues avant de les utiliser.

3. Pourquoi est-il dangereux d'afficher **tel quel** ce que l'utilisateur envoie ?

   > Parce qu'un utilisateur peut envoyer du code malveillant qui pourrait être exécuté sur la page. Il faut donc sécuriser les données avant de les afficher.

---

## 🟣 Exercice 8 — Les formulaires

1. Quelle est la différence visible entre GET et POST ?

   > Avec GET, les informations apparaissent dans l'URL. Avec POST, elles ne sont pas visibles dans l'adresse du site.

2. Pour un formulaire de **recherche**, quelle méthode choisiriez-vous ? Et pour un formulaire de **connexion avec mot de passe** ? Pourquoi ?

   > Pour une recherche, je choisirais GET, car les mots recherchés apparaissent dans l'URL. Pour une connexion, je choisirais POST pour ne pas afficher le mot de passe dans l'adresse du site.

3. Les données envoyées en POST sont-elles vraiment « secrètes » ? (Pensez à ce que vous avez vu dans l'onglet Réseau.)

   > Non, car on peut quand même voir les données dans l'onglet Réseau du navigateur. Pour les protéger, il faut utiliser HTTPS, qui chiffre les informations pendant leur envoi.

---

## 🔴 Exercice 9 — Les codes de statut

1. Quelle est la différence entre une erreur `4xx` et une erreur `5xx` ? Qui est « fautif » dans chaque cas ?

   > Une erreur 4xx vient généralement d'un problème dans la demande de l'utilisateur (page introuvable, accès interdit). Une erreur 5xx vient d'un problème sur le serveur.

2. Comment fonctionne une redirection ? Qui fait la deuxième requête : le serveur ou le navigateur ?

   > Le serveur indique au navigateur une nouvelle adresse où aller. C'est ensuite le navigateur qui fait une deuxième requête vers cette adresse.

3. Donnez un exemple de situation où un vrai site utilise une redirection.

   > Quand on tape une ancienne adresse d'un site, celui-ci peut nous rediriger automatiquement vers sa nouvelle adresse.

---

## 🔴 Exercice 10 — Ce que le serveur sait de vous

1. Citez trois informations que le serveur connaît sur vous, sans que vous ayez rien rempli.

   > Mon adresse IP, le type de navigateur que j'utilise et mon système d'exploitation.

2. À quoi peut servir l'en-tête `Accept-Language` pour un site comme Wikipédia ?

   > Il permet de connaître la langue préférée du visiteur pour lui afficher directement Wikipédia dans la bonne langue.

3. Dans l'Access log, retrouvez une requête qui a reçu un code `404`. Quelle page était demandée ?

   > Une page ou un fichier qui n'existe pas sur le serveur était demandé.

4. Après cet exercice, que pensez-vous de la notion de « navigation anonyme » ?

   > Je pense qu'on n'est jamais totalement anonyme sur Internet, car les sites peuvent récupérer plusieurs informations sur nous, même sans qu'on les donne directement.

---

## 🔴 Exercice 11 — Le Web des machines : API et JSON

1. Quelle est la différence entre une page HTML et une réponse JSON ? À qui chacune est-elle destinée ?

   > Le HTML sert à afficher une page pour les humains, tandis que le JSON sert à échanger des données entre les machines et les applications.

2. Dans la page `/horloge`, quel code s'exécute sur le **serveur** et quel code s'exécute dans le **navigateur** ?

   > Le code Python s'exécute sur le serveur pour récupérer l'heure. Le JavaScript s'exécute dans le navigateur pour afficher l'heure sur la page.

3. Citez une application de votre téléphone qui, selon vous, utilise une API. Quelles données échange-t-elle ?

   > L'application météo utilise une API. Elle récupère des informations comme la température, la pluie et les prévisions météo pour les afficher sur mon téléphone.

---

## 🏁 Pour conclure

En quelques phrases, expliquez à un ami ce qui se passe entre le moment où il tape une adresse dans son navigateur et celui où la page s'affiche :

> Quand je tape une adresse dans mon navigateur, celui-ci envoie une demande au serveur pour récupérer la page. Le serveur reçoit la demande et renvoie les fichiers nécessaires (HTML, CSS, images, etc.). Ensuite, le navigateur lit ces fichiers et affiche la page à l'écran. Tout cela se passe en quelques secondes grâce à Internet.
