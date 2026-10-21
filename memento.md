# Memento TP Terminale

## Étape 1  - Se repérer : 
* Affichez le chemin du dossier courant : pwd
* Affichez son contenu : ls
* Les fichiers cachés : ls -a 
* Version longue sans les fichiers
cachés : ls -l
* Version longue avec les fichiers cachés : ls -la
* Affichez l'aide de la commande ls : man ls
* Déplacez-vous dans votre dossier Documents : cd documents 
* Affichez son contenu : ls

## Étape 2 - Organiser un projet :

* Créez le dossier station-meteo : mkdir station-meteo
* cd station-meteo
* Depuis ce dossier et en une seule commande, le
dossier brouillon et son sous-dossier data:
mkdir -p brouillon/data
* créez en une seule commande les dossiers src , tests et docs à la racine de
station-meteo : mkdir src tests docs
* créez dans brouillon un fichier main.py contenant la ligne
print("Station météo prête") ; :
* echo 'print("Station météo prête");' > brouillon/main.py
* déplacez main.py dans src : mv brouillon/main.py src/
* puis le dossier data et son contenu à la racine de
station-meteo : mv brouillon/data ./
* Supprimez le dossier brouillon : rm -r brouillon
* exécutez src/main.py avec Python : python3 main.py

## Étape 3 - Manipuler le contenu des fichiers :

* créez fichier1.txt contenant Bonjour ! et fichier2.txt contenant Je m'appelle Antony : echo "Bonjour" > fichier1.txt
* echo "Je m'appelle Antony" > fichier2.txt 
* créez resultat.txt en concaténant les deux fichiers, puis affichez-le : cat fichier1.txt fichier2.txt > resultat.txt 
*  ajoutez la ligne Fin du test. à la fin de resultat.txt sans effacer son contenu : echo "Fin du test." >> resultat.txt
* copiez resultat.txt en resultat_sauvegarde.txt : cp resultat.txt resultat_sauvegarde.txt

## Étape 4 -  Retrouver et quitter :
Affichez la liste des dernières commandes tapées : 
* 181  cd ..
* 182  ls
* 183  cd docs
* 184  echo "Bonjour" > fichier1.txt
* 185  ls
* 186  echo "Je m'appelle Antony" > fichier2.txt

Nous avons utilisé la commande history
 
 Retrouvez une commande précédente avec le clavier, sans la retaper :
 * cat resultat_sauvegarde.txt

Nous avons utilisé la flèche du haut

Depuis Documents , retrouvez tous les fichiers .py contenus dans station-meteo :
* station-meteo/src/main.py

Nous avons utilsé la commande : 
 * find station-meteo -name "*.py"

 Quittez le terminal.
 * Nous avons utilisé la commande exit
