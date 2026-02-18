Cette application est l'exemple parfait pour comprendre comment gérer des données qui changent. On appelle cela une application "Compteur".

<img width="1920" height="1080" alt="Screenshot (114)" src="https://github.com/user-attachments/assets/1f5e21b3-86b1-4f96-8a4c-ed2fc8d5788d" />
<img width="1920" height="1080" alt="Screenshot (113)" src="https://github.com/user-attachments/assets/1dd5a231-300e-4104-b66c-733877cf0472" />

* Explication des composants :

  1. La mémoire de l'application (La Variable)
int _counter = 0; : C'est une petite boîte qui stocke un nombre entier. Au début, elle vaut 0.

Chaque fois que vous cliquez, on change ce nombre avec _increment (+1) ou _decrement (-1).

2. Le signal de mise à jour (setState)
C'est la partie la plus importante de Flutter :

Quand vous appelez setState, vous dites à Flutter : "Le nombre a changé ! Re-dessine l'écran tout de suite pour afficher la nouvelle valeur." * Sans setState, le nombre changerait dans la mémoire, mais l'utilisateur verrait toujours l'ancien chiffre à l'écran.

3. L'apparence interactive
Actions dans l'AppBar : Le petit bouton "rafraîchir" en haut à droite pour remettre le compteur à zéro.

Boutons colorés : Utilisation de ElevatedButton.styleFrom pour mettre le bouton "Augmenter" en vert et "Diminuer" en rouge.

Sécurité : Le code empêche le compteur de descendre en dessous de zéro grâce à la condition if (_counter > 0).

* Capture de l'app :

<img width="1920" height="1080" alt="Screenshot (97)" src="https://github.com/user-attachments/assets/6fc8ef8a-e5c3-47a5-a7ea-d6da1e5ac962" />

