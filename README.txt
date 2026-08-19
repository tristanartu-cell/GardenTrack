Mon Potager — installation PWA

Le fichier HTML original n’a pas été trouvé dans l’environnement disponible : seul un fichier image était présent dans /mnt/user-data/uploads/.

Placez icon-192.png, icon-512.png et manifest.json dans le même dossier que votre fichier HTML (à la racine publiée par GitHub Pages). Dans la section <head> de l’HTML existant, ajoutez exactement :

<link rel="manifest" href="manifest.json">
<meta name="theme-color" content="#2e7d32">
<link rel="apple-touch-icon" href="icon-192.png">

Vérifiez également que le viewport est présent (s’il ne l’est pas déjà) :

<meta name="viewport" content="width=device-width, initial-scale=1">

Publiez ensuite les trois fichiers image/JSON avec l’HTML sur GitHub Pages. Sur Android/Chrome, ouvrez la page publiée puis utilisez le menu ⋮ → « Ajouter à l’écran d’accueil » (ou « Installer l’application »).
