DeyClient 1.0.31

DeyClient est un client utilitaire pour Minecraft 1.21.1 / NeoForge, conçu pour centraliser Baritone, des automatisations, des outils de combat et des fonctions de rendu dans une interface compacte.

L'objectif est de rendre les tâches répétitives beaucoup plus simples à configurer et à contrôler, sans avoir à mémoriser toutes les commandes Baritone.

BARITONE

DeyClient fournit une interface graphique permettant de contrôler Baritone sans avoir à taper manuellement les commandes.

⛏️ Mine

Sélection des blocs à miner automatiquement.

Sélection de blocs
Plusieurs blocs sélectionnables
Quantité configurable
0 = minage infini
Contrôle directement transmis à Baritone
📍 Goto

Déplacement automatique vers des coordonnées :

X
Y
Z

Baritone calcule ensuite automatiquement le chemin.

👤 Follow Player

Permet de suivre automatiquement un joueur.

Détection des joueurs actuellement connectés
Sélection directement dans DeyClient
Aucun pseudo à saisir manuellement

🏗️ Build

Interface simplifiée pour lancer les fonctions de construction Baritone.

🌍 Locate

Recherche de structures Minecraft.

DeyClient tente d'abord la commande vanilla /locate.

Si celle-ci est indisponible ou si le joueur n'a pas les permissions nécessaires, DeyClient peut automatiquement :

Explorer avec Baritone → scanner les chunks chargés → détecter des signatures de structures → se déplacer vers la structure détectée.

Structures reconnaissables notamment :

Villages
Strongholds
Ancient Cities
Trial Chambers
Bastions
Nether Fortresses
End Cities
Ocean Monuments
Woodland Mansions
Pillager Outposts
Desert Pyramids
Mineshafts
Shipwrecks

La détection sans /locate est heuristique et peut donc occasionnellement produire des faux positifs.

🌳 AutoWood V2

Récolte automatique du bois.

Sélection des types de bois
Quantité configurable
0 = récolte infinie

🌾 Farm V2

Système de farming configurable basé sur Baritone.

Rayon de farm configurable
Centre sur la position actuelle
Centre sur un waypoint DeyClient
Replantation automatique des cultures
Replantation du Nether Wart
Déplacement automatique vers la ferme
Start / Stop
⏯️ Contrôle Baritone

Commandes rapides :

Pause
Resume
Stop
⚙️ AUTOMATION

🎣 AutoFish

Automatise la pêche.

🍗 AutoEat

Mange automatiquement lorsque nécessaire tout en évitant de bloquer l'utilisation normale du clic droit.

🛠️ AutoTool

Sélection automatique de l'outil approprié.

🛡️ ToolSaver

Évite d'user inutilement les outils fortement endommagés.

🔥 AutoTorch V2

Pose automatiquement des torches lorsque la luminosité devient trop faible.

Paramètres :

Niveau de lumière
Délai entre les poses

⛏️ AutoMine

Automatisation du minage du bloc situé devant le joueur.

🌉 AutoBridge

Aide à la construction automatique de ponts.

🔄 AutoReconnect

Reconnecte automatiquement le joueur après une déconnexion.

Délai configurable

📦 AutoRefill

Recharge automatiquement les stacks utilisés depuis l'inventaire.

Seuil de déclenchement configurable

💤 Anti-AFK

Évite les déconnexions AFK avec des actions légères et périodiques.

Intervalle configurable
Petite rotation
Animation de main
Pas de déplacement forcé permanent

❤️ SAFETY

🏃 AutoEscape

Système de fuite automatique lorsque la vie descend sous un seuil défini.

Deux modes :

FLEE

Détecte la menace proche et tente de s'en éloigner.

WAYPOINT

Interrompt l'action Baritone actuelle puis rejoint automatiquement un waypoint de sécurité.

Le seuil de vie est configurable.

🗿 AutoTotem

Équipe automatiquement un Totem of Undying lorsque l'offhand est vide.

DeyClient ne remplace volontairement pas :

Bouclier
Nourriture
Objet déjà tenu en offhand

✨ AutoMending

Aide à réparer automatiquement l'équipement possédant Mending.

DeyClient :

détecte les orbes d'XP proches ;
recherche les objets Mending endommagés dans la hotbar ;
privilégie l'objet ayant le plus besoin d'être réparé ;
sélectionne temporairement cet objet ;
restaure ensuite le slot précédent.

👁️ RENDER

☀️ FullBright

Augmente fortement la visibilité dans les zones sombres.

📊 HUD

Affiche différentes informations directement à l'écran :

Coordonnées XYZ
Direction
FPS
Modules actifs

👁️ ESP V2

Affichage des entités avec filtres :

Joueurs
Ennemis
Alliés

Distance configurable.

📋 ESP Info HUD

Liste compacte des entités détectées.

Les mobs identiques sont automatiquement regroupés :

Zombie ×5 • 12m
Skeleton ×2 • 18m

Les joueurs restent affichés individuellement avec :

Pseudo
Distance
Vie

📦 Container ESP

Détection des conteneurs dans les chunks chargés.

Distance configurable.

💎 X-Ray

Mode de visualisation destiné à faciliter la recherche de blocs à travers le terrain.

🕳️ Cave Finder

Aide à identifier les zones souterraines et cavités.

🏹 Arrow Trajectory

Affiche une estimation de la trajectoire des flèches.

⚔️ COMBAT

⚔️ KillAura

Attaque automatiquement les cibles correspondant aux filtres sélectionnés.

🎯 Aimbot

Assistance à la visée pour le combat rapproché.

🏹 Bow Aimbot

Assistance à la visée avec arc utilisant une estimation balistique de la trajectoire.

🛡️ AutoBlock

Automatisation de l'utilisation du bouclier.

Filtres de cible

Les modules Combat peuvent distinguer :

Joueurs
Mobs hostiles
Alliés

📍 WAYPOINTS

DeyClient possède son propre système de waypoints.

Il permet de :

Sauvegarder la position actuelle
Nommer un waypoint
Rejoindre automatiquement un waypoint avec Baritone
Utiliser un waypoint comme destination AutoEscape
Utiliser un waypoint comme centre de Farm
Utiliser un waypoint dans Job Manager
Supprimer un waypoint

Les waypoints sont sauvegardés dans la configuration DeyClient.

🤖 JOB MANAGER

L'un des systèmes d'automatisation avancés de DeyClient.

Il permet de créer des boucles de travail autonomes.

Jobs disponibles
WOOD
MINE
FARM

Exemple :

MINER
↓
Inventaire plein
↓
Retour waypoint
↓
Coffre
↓
Dépôt automatique
↓
Retour au travail
↓
MINER

Le cycle peut fonctionner en boucle.

📦 AutoDeposit

DeyClient peut enregistrer un coffre/conteneur comme destination.

Lorsque l'inventaire est plein :

Baritone s'arrête.
DeyClient rejoint le waypoint de retour.
Il rejoint le conteneur enregistré.
Il ouvre le conteneur.
Les ressources sont déposées.
Le job reprend automatiquement.

Certains objets utiles sont protégés du dépôt automatique, notamment :

Outils
Armures
Totems
Torches
Nourriture
Bouclier
Arc
Arbalète
Elytra
Canne à pêche
Cisailles
Briquet
🚶 Modes de déplacement
NORMAL

Baritone peut casser et poser des blocs.

SAFE

Baritone peut poser des blocs mais évite d'en casser.

CLEAN

Pas de casse ni de pose pendant le déplacement.

🌾 JOB FARM

Le Job Manager peut également gérer une ferme.

Deux waypoints différents peuvent être définis :

CHAMP
↓
Farm automatique
↓
Inventaire plein
↓
RETOUR / COFFRE
↓
Dépôt
↓
Retour au CHAMP
↓
Farm
🎛️ PROFILES

Plusieurs profils permettent de modifier rapidement la configuration du client :

⛏️ MINING
🌍 EXPLORE
⚔️ COMBAT
🛡️ SAFE
CUSTOM
⌨️ KEYBINDS

Les principales fonctions de DeyClient peuvent recevoir une touche personnalisée.

Catégories :

Baritone
Automation
Combat
Render

Un système UNBIND permet de sélectionner une fonction puis de supprimer son raccourci.

Plusieurs modules peuvent également partager la même touche.

🚨 STOP ALL

Un bouton d'urgence permet d'arrêter rapidement :

Baritone
Jobs
Automatisations actives
Actions contrôlées par DeyClient

💾 CONFIGURATION

DeyClient possède une configuration persistante.

Sont notamment sauvegardés :

Modules activés
Paramètres
Keybinds
Waypoints
Profils
Position de la fenêtre
Dernier menu utilisé
Paramètres Job Manager
Paramètres Farm
Paramètres Render

🖥️ INTERFACE

Interface ClickGUI compacte conçue spécialement pour DeyClient.

Thème sombre
Accents bleu/violet
Interface déplaçable
Position sauvegardée
Pas de blur Minecraft derrière l'interface
Navigation par catégories
Interface compacte
HUD indépendant

Ouverture du menu :

Right Shift

📥 Installation

L'installation manuelle nécessite actuellement :

Minecraft 1.21.1
NeoForge
Java 21
Baritone 1.11.2 NeoForge
Le JAR DeyClient

Placez les mods dans :

.minecraft/mods/

Un DeyClient Installer est également en développement afin d'automatiser l'installation de DeyClient et de la version correspondante de Baritone.

🚧 Roadmap

Le projet est toujours en développement.

Parmi les objectifs :

Support de plusieurs versions Minecraft
Installer Windows autonome
Détection automatique des versions installées
Gestion des mises à jour
Amélioration du Job Manager
Amélioration de Farm V2
Amélioration du système Locate sans permissions
Nouveaux modules d'automatisation
Amélioration de l'ESP
Interface encore plus configurable

⚠️ Disclaimer

DeyClient est un projet indépendant et n'est pas affilié à Mojang, Microsoft, NeoForge ou Baritone.

Certaines fonctionnalités peuvent être interdites par les règles de certains serveurs Minecraft. Il appartient à l'utilisateur de respecter les règles du serveur sur lequel il joue.

💜 By Deyron

DeyClient — automate the boring stuff.
