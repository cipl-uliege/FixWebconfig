# FixWebconfig
Installer sur le serveur "URL Rewrite Module 2.1" grâce au lien dans download.txt. (j'ai téléchargé personnellement => French: x64 installer)
<br>
Remplacer index.html dans wwwroot par celui-ci donné ici.
<br>
Placer le web.config donné ici dans wwwroot à la même racine que index.html.

<br>
<b>Pourquoi ?</b>
<br>
Si on essaye d'aller directement sur "http://cipl-cloud45.segi.ulg.ac.be/search/category" qui est une URL valide, il nous sortira une 404 not found. Car il essaye d'aller dans le dossier search puis category qui tout deux n'existent pas. Le web.config sert juste à rediriger toutes les URLs vers index.html en gardant l'URL intact pour qu'ensuite React puisse l'interpréter et faire correctement son routing.
