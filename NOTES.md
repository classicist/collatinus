# Collatinus-11, notes

lundi 4 janvier 2016 

## COMPILATION
Requis :
- Un compilateur C++ ;
- Les bibliothèques Qt 5.\*
- Ajuster le PATH de la machine pour que
  compilateur et bibliothèques soit accessibles
  depuis le répertoire de développement ;
- En ligne de commande :
  * $ qmake
  * $ make
- Créer les répertoires bin/, bin/data et bin/data/dicos
- Placer dans bin/data/ les lexiques téléchargeables 
  [à l'adresse](http://outils.biblissima.fr/collatinus/)
- Placer dans bin/data/dicos les dictionnaires xml et
  djvu les dictionnaires téléchargeables à la même adresse ;
- Lancer Collatinus en ligne de commande :    
  * $ cd bin
  * $ ./collatinus    
  ou après avoir installé un raccourci.

## BOGUES ET PROBLÈMES
- Flexion de moenia, ium. Vérifier les modèles pluriels.
- Flexion de multus et ses degrés allogènes (plus, plurimus)
- flexion de facio et fio, et des composés

## À FAIRE :
- Dans le presse-papier, insérer une signature "édité avec C11+url";
  idem pour l'impression ?
- Nettoyage des -pte -met -quoi dans les traductions ;
- chargement des lexiques et dictionnaires, compressés,
  prêts à être décompressés et installés par Collatinus.
- Modèles :
  *	Vérifier les modèles ;
  *	Traiter les noms 3ème decl pl. majores, orum, donné sing. ;
  * modèles nolo et malo ;
  * Vérifier facio et fio ;
  *	Construire des modèles passifs/intransitifs.
- Système d'hyperliens dans les résultats, qui permet d'afficher
  des entrées. Par exemple, le lemme multus donne ses degrés par
  un hyperlien vers plus, pluris, et vers plurimus, a, um.

## Branche maj
Branche de mise à jour des lexiques.
- Créer un dépôt distant,
- Dans le dépôt, des fichiers compressés, et une page d'accueil et des liens ;
- Dans Collatinus, menu Lexique ou Aide, ou les deux, une option màj ;
- Créer le dialogue maj 
  * lien vers le dépôt, mode d'emploi ;
  * Un bouton qui lance un QFileDialog de sélection des fichiers téléchargés ;
  * Un bouton OK pour lancer la décompression et copie des fichiers ;
  * Un bouton Annuler.

## DOC
- Un modèle d'utilisation des docks est dans les exemples Qt5 : 
  ${Doc-qt5}/examples/widgets/mainwindows/dockwidgets