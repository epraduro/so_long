<h2/>Projet — so_long </h2>
<p align="center"> <img src="https://img.shields.io/badge/42-Project-black?style=for-the-badge&logo=42"> <img src="https://img.shields.io/badge/Language-C-blue?style=for-the-badge&logo=c"> <img src="https://img.shields.io/badge/Graphics-MiniLibX-orange?style=for-the-badge"> </p>

<h2/> Description </h2>

so_long est un petit jeu 2D développé en C dans le cadre du cursus 42, utilisant la bibliothèque graphique MiniLibX.

<h2/> Objectifs du projet : </h2>

•	Gestion de fenêtres et d’événements </br>
•	Rendu graphique avec MiniLibX </br>
•	Manipulation de maps </br>
•	Gestion de mémoire (sans fuites) </br>
•	Bases de la logique de jeu </br>

<h2/> Gameplay </h2>

•	Le joueur se déplace dans une carte 2D </br>
•	Il doit récupérer tous les collectibles </br>
•	Une fois tous les objets récupérés, la sortie devient accessible </br>
•	Le jeu se termine lorsque le joueur atteint la sortie </br>

<h2/> Contrôles </h2>

| Touche / Flèches  | Action       |
| ------- | ------------ |
| <p align="center"> W / ↑ </p>   | <p align="center"> ⬆️ Monter </p>   |
| <p align="center"> A / ← </p>  | <p align="center"> ⬅️ Gauche </p>   |
| <p align="center"> S / ↓ </p>  | <p align="center"> ⬇️ Descendre </p> |
| <p align="center"> D / → </p>  | <p align="center"> ➡️ Droite </p>   |
| <p align="center"> ESC / Q </p> | <p align="center"> ❌ Quitter </p>   |

<h2/> Format des maps </h2>

Les maps doivent être au format .ber et respecter les règles suivantes :

<h4> • Caractères autorisés: </h4>

| Symbole | Signification |
| ------- | ------------- |
| <p align="center"> `1` </p>    | <p align="center"> Mur </p>          |
| <p align="center"> `0` </p>    | <p align="center"> Sol </p>          |
| <p align="center"> `C` </p>    | <p align="center"> Collectible </p>  |
| <p align="center"> `E` </p>    | <p align="center"> Sortie </p>       |
| <p align="center"> `P` </p>    | <p align="center"> Joueur </p>       |

<h4> • Contraintes: </h4>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;-	Map rectangulaire </br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;-	Entourée de murs (1) </br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;-	Doit contenir : </br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;•	au moins 1 sortie </br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;•	au moins 1 collectible </br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;•	exactement 1 joueur </br>

<h2/> Installation </h2>

<h4/> Prérequis </h4>
•	GCC </br>
•	Make </br>
•	MiniLibX </br>

<h4/> Compilation </h4>
	
	make

Version bonus: 

	make bonus

<h2> Lancer le jeu </h2>

	./so_long maps/map.ber

Version bonus:

	./so_long_bonus maps/map.ber


<h2> Tests </h2>

<h4> Tu peux tester : </h4>

• Collisions avec les murs </br>
• Comptage des mouvements </br>
• Gestion des erreurs de map </br>
• Fuites mémoire avec Valgrind </br>

<h2> Structure du projet </h2>

	.
	├── bonus/
	├── gnl/
	├── image_xpm/   # Textures
	├── minilibx/    # Librairie graphique
	├── Makefile
	└── README.md

<h2> Bonus </h2>

•	Animations <br/>
•	Compteur de pas à l’écran <br/>
