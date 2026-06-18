# Téléchargement

Pour commencer, téléchargez Chocolatine depuis Github 

[Download Chocolatine](https://github.com/Louloubiwan/Chocolatine){ .md-button .md-button--primary }



## Windows

Sur Windows, exécutez `chocolatine.exe`

##  Linux

Sur Linux, exécutez `./chocolatine`

/!\ Si vous avez cette erreur /!\ :

* `error while loading shared libraries : libedit.so.0 cannot open shared objectfile`

Then  : 

* `sudo apt install build-essential`

* `sudo ln -s /usr/lib/x86_64-linux-gnu/libedit.so.2 /usr/lib/x86_64-linux-gnu/libedit.so.0`




Pour commencer à utiliser Chocolatine, n’oubliez pas de consulter la documentation : 

[Documentation](documentation.md){ .md-button .md-button--primary }




------------------------------------------------------

# Compiler Chocolatine (POUR DEVELOPPEURS SEULEMENT)

## Installer GCC sur Linux

Le compilateur GCC est déjà installé par défaut sur Linux (normalement) ; si jamais ce n'est pas le cas, exécutez cette commande-

  *  `sudo apt install build-essential`

## Installer GCC sur Windows

[Windows download link](https://sourceforge.net/projects/mingw-w64/)



## Compiler Chocolatine

Pour vérifier que GCC est installé sur votre ordinateur, exécutez cette commande :

  *  `gcc --version`



Une fois à la racine du projet, exécutez cette commande pour compiler Chocolatine :

 * `gcc -std=c99 -Wall chocolatine.c mpc.c -o chocolatine1`


Après cela, l’exécutable `chocolatine1` devrait apparaître dans le dossier.

