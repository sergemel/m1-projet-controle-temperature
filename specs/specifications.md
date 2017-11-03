# Suivit et contrôle de température : Mise en oeuvre
## L'historique des températures mesurées

### E 3.1 : l'unité de température dépend du pays d'installation

#### Spécification fonctionnelle détaillée :

Les calculs et la sauvegarde de température se font en Kelvin.  
L'unité d'affichage est choisie à l'installation, c'est degré Celsius (°C) Fahrenheit (°F).  
On peut modifier l'unité d'affichage de Celsius <-> Fahrenheit.  
A l'installation, le système demande à choisir le pays d'installation dans une liste déroulante des pays. Tous les pays sont en degré Celsius (°C) sauf aux Etats-Unis, au Bélize et aux Îles caïman  Fahrenheit (°F).  

Auteur : Quentin lechat
Relecteur : Guillaume Lamanda

#### Spécification technique :

On ajoute la classe Configuration :
- Un attribut « userTemp » correspondant à l’unité de température en booléen. Le faux correspond au Celcius et le vrai correspond Fahrenheit (+ getter/setter),
Classe APISuivi : 
- Une méthode « LireTemperature », qui permet de récupérer la température en via la méthode existante « lireTempérature » de la classe SuiviChauffage puis la convertie via la méthode « conversion »,
- Une méthode AjoutNouvelleMesure
- Une méthode « conversion » qui permet de convertir la valeur depuis le Kelvin à l’unité de destination choisi par l’utilisateur.  

Autheur : Guillaume Lamanda  
Relecteur : Serge Mel

#### Plan de test : 
A faire par Mel

#### Réalisation : 
A faire par Zak