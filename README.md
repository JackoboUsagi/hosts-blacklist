# hosts-blacklist
Blocage des sites Web sur Windows 11

- Etape 1 : Enregistrer ce fichier "hosts" dans C:\Windows\System32\drivers\etc
- Etape 2 : Ouvrir un invite de commandes
- Etape 3 : Exécuter les commandes suivantes
``
ipconfig /flushdns
nbtstat -R
``
- Etape 4 : Nettoyer le cache des navigateurs Web


Pour tester le blocage, utiliser les commandes suivantes
``
ping -4 www.example.com -n 1
ping -6 www.example.com -n 1
ping -4 example.com -n 1
ping -6 example.com -n 1
``

Vous devriez avoir le message suivant :
``
La requête Ping n’a pas pu trouver l’hôte www.bfmtv.com. Vérifiez le nom et essayez à nouveau.
``

