# Ionic 3 climbing list app

Ce projet est issu du template "tab-starter" disponible nativement avec Ionic avec des components additionnels. Il contient notamment un appel à un fichier JSON (base de données de l'application), appelé par HTML.
De plus, un systeme de recherche est implémenté via un loader qui laisse apparaitre les données filtrées. 


## Getting Started

Pour commencer à utiliser cette application; vous devez choisir entre:
      - Download la derniere release du projet au format zip ici :  https://github.com/goslowone/ValentinMIGNARD_M2FIC_VTI_Ionic
      - Cloner le repository via la commande : $ git clone https://github.com/goslowone/ValentinMIGNARD_M2FIC_VTI_Ionic.git


### Project Structure
```
.
 ├── resources                    # Build les fichiers pour les plateformes spécifique (iOS, Android) 
 ├── src                          # Le dossier main de l'application, où vivent les fichiers principaux
 ├── config.xml                   # Fichier de config Ionic
 ├── package.json                 # Dependance et builds des scripts
 ├── readme.md                    # Description du projet et help
 ├── tsconfig.json                # Configurations TypeScript
 └── tslint.json                  # TypeScript linting options
```

#### src directory
```
.
   ├── ...
   ├── src                       
   │   ├── app                    # Ce dossier contient les modules globaux et le style
   │   ├── assets                 # Ce dossier contient des images et le fichier * data.json * (BDD du projet)
   |   ├── pages                  # Contient toutes les pages individuelles (home, tabs, category, list, single-item)
   |   ├── services               # Contient la item-api service qui récupere les datas du fichier JSON
   |   ├── theme                  # les variables globales SCSS à utiliser dans l'application
   |   ├── declarations.d.ts      # Un fichier de configuration pour rendre les objets TypeScript disponibles
   |   ├── index.html             # Le fichier d'index racine - celui qui lance l'application.
   |   ├── manifest.json          # Metadata de l'app
   │   └── service-worker.js      # Fichier de configuration cache
   └── ...
```


##### Start the project
```
Le projet se lance avec les commandes basiques d'Ionic

1. Ouvrir un invide de commande unix de type terminal.
2. Run la commande : 'npm install' pour installer dans le dossier 'node_modules' toutes les dépendance liées au projet.
3. Run 'ionic serve' pour démarrer l'application.
4. Pour build le projet de façon a être utilisé sur mobile, run : 
      - 'ionic build android' pour un mobile Android
      - 'ionic build ios' pour un mobile IOS (à privilégier sur MacOs).

Une alternative consiste à émuler l'application sur un appareil ou à l'uploader sur le ionic cloud. À partir de là, vous pouvez télécharger l'application ionic view et l'utiliser sur tous les appareils.
```

###### Plugins
```
UI et back components utilisés dans cette application:
      - List : avec les balises "ion-list" et "ion-avatar" pour les images 
      - Item : avec les balises "ion-item" et "ion-label"
      - Tabs : avec la balise "ion-tabs" permettant de faire plusieurs onglets (ici Home et Search)
      - Platform : pour détecter la pateforme (mobile ou ordinateur) et ainsi adapter l'affichage de façon optimale
      - SplashScreen
      - StatusBar 
```