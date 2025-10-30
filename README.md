# 🐍 TP 1 – Découverte de Python avec Thonny

## 🌟 Objectif du TP

Apprendre à écrire, exécuter et comprendre ses premiers programmes Python en traduisant des **algorithmes classiques** déjà vus en pseudo-code.

---

## 🧰 1. Installation de l’environnement Thonny

### Étapes :

1. Rendez-vous sur : [https://thonny.org/](https://thonny.org/)
2. Téléchargez **Thonny with Python included** (Windows) ou la version adaptée à votre système.
3. Installez avec les options par défaut.
4. Lancez Thonny :

   * Zone blanche = code
   * Zone du bas = console Python
   * Bouton ▶️ = exécuter

---

## 🧑‍💻 2. Premiers pas avec Python

### Exemple minimal :

```python
print("Bonjour le monde !")
```

Appuyez sur **▶️** pour exécuter le code.

---

## 🧩 3. Les bases du langage Python

### 📦 Les variables

```python
nom = "Alice"
age = 20
```

### 💬 L’affichage

```python
print("Bonjour", nom)
```

### ⌨️ La saisie au clavier

```python
nom = input("Entrez votre nom : ")
```

> Pour les nombres : `int(input(...))` ou `float(input(...))`

### ⚙️ Les conditions

```python
if condition:
    # bloc d’instructions (indenté de 4 espaces)
```

> En Python, **l’indentation (les espaces)** remplace les accolades et mots-clés comme “finsi”.

### 🔁 Les boucles

```python
for i in range(1, 6):
    print(i)

# ou

i = 1
while i <= 5:
    print(i)
    i += 1
```

---

## 🗂️ 4. Organisation du TP

Créez un dossier : `TD01_Python/`
Chaque exercice = un fichier : `exo01.py`, `exo02.py`, etc.

---

# 🧠 Partie 2 – Exercices Python guidés par le pseudo-code

Chaque exercice est issu de votre TD d’algorithmique.
On vous fournit le **pseudo-code corrigé** : à vous de le **traduire en Python**.

---

## 🧮 Exercice 1 – Trace d’un programme

**Pseudo-code :**

```
si (A = B ou A <> C) et (B <> C) alors
   A ← B – C
   si A < B alors
      B ← A
      C ← 3
   sinon
      A ← B
   finsi
   C ← 2 * C
sinon
   A ← 2 * C
finsi
```

🎯 **Tâche :** Demandez A, B, C à l’utilisateur et traduisez cet algorithme en Python.
Affichez ensuite les valeurs finales.

---

## 🧑‍🤝‍🧑 Exercice 2 – Bonjour Madame / Monsieur

**Pseudo-code :**

```
programme sexe
   nom : chaine
   sexe : caractère
   debut
      afficher "Entrer votre nom"
      saisir nom
      afficher "Sexe (F/M)"
      repeter
         saisir sexe
      jusqu'à sexe = "F" ou sexe = "M"
      si sexe = "F" alors
         afficher "Bonjour Madame", nom
      sinon
         afficher "Bonjour Monsieur", nom
      finsi
   fin
```

🎯 **Tâche :** Reproduisez ce comportement en Python avec une boucle `while` et `input()`.

---

## 🔣 Exercice 3 – Logique conditionnelle

**Pseudo-code exemple :**

```
"Les valeurs X et Y sont toutes deux supérieures à 3"  →  X>3 et Y>3
```

🎯 **Tâche :** Écrivez et testez les expressions suivantes en Python :

1. X, Y, Z sont identiques
2. X, Y, Z sont identiques mais différents de T
3. X est entre Y et T
4. Deux valeurs seulement sont identiques parmi X, Y, Z

---

## 🏙️ Exercice 4 – Ville et habitants

**Pseudo-code :**

```
programme habitants
   ville : chaîne
   nbhab : entier
   debut
      afficher "entrez un nom de ville"
      saisir ville
      afficher "entrez le nombre d'habitants"
      saisir nbhab
      afficher ville, " possède ", nbhab, " habitants"
   fin
```

🎯 **Tâche :** Traduisez ce programme en Python avec `input()` et `print()`.

---

## 💶 Exercice 5 – Conversion Euro/Franc

**Pseudo-code :**

```
programme conversion
   prix : numérique
   debut
      afficher "entrez un prix en Euro"
      saisir prix
      afficher prix * 6.55957
   fin
```

🎯 **Tâche :** Demandez un prix en euros et affichez le montant converti.

---

## 📊 Exercice 6 – Moyenne et message

**Pseudo-code :**

```
si moyenne >= 10 alors
   afficher "passage"
sinon
   si moyenne >= 8 alors
      afficher "redoublement"
   sinon
      afficher "exclusion"
   finsi
finsi
```

🎯 **Tâche :** Saisissez une moyenne et traduisez cette logique en Python.

---

## 🚦 Exercice 7 – Feu tricolore du robot

**Pseudo-code :**

```
programme robot
   couleur : chaîne
   debut
      afficher "entrez une couleur (rouge/orange/vert)"
      repeter
         saisir couleur
      jusqu'à couleur = "rouge" ou "orange" ou "vert"
      cas de couleur
         "rouge" : afficher "s'arrêter"
         "orange" : afficher "ralentir"
         "vert" : afficher "passer"
      fincas
   fin
```

🎯 **Tâche :** Reproduisez ce comportement en Python.
Utilisez une boucle `while` et des `if / elif / else`.

---

## 🧮 Exercice 8 – Moyenne de plusieurs notes

**Pseudo-code :**

```
programme moyenne
   note, cumul, nb : numérique
   rep : caractère
   debut
      cumul ← 0
      nb ← 0
      repeter
         afficher "entrer une note"
         saisir note
         cumul ← cumul + note
         nb ← nb + 1
         afficher "voulez-vous continuer ? (O/N)"
         repeter
            saisir rep
         jusqu’à rep="O" ou rep="N"
      jusqu’à rep="N"
      afficher cumul/nb
   fin
```

🎯 **Tâche :** Traduisez ce programme avec une boucle `while` et un compteur.

---

## ➕ Exercice 9 – Compter positifs et négatifs

**Pseudo-code :**

```
pour i de 1 à 20
   saisir valeur
   si valeur >= 0 alors
      positif ← positif + 1
   finsi
finpour
```

🎯 **Tâche :** Traduisez ce code en Python avec une boucle `for`.

---

## 🧾 Exercice 10 – Note min et max

**Pseudo-code :**

```
min ← 20
max ← 0
pour k de 1 à 30
   saisir note
   si note > max alors max ← note
   si note < min alors min ← note
finpour
```

🎯 **Tâche :** Écrivez le programme Python correspondant.

---

## 🌡️ Exercice 11 – Températures de l’année

**Pseudo-code :**

```
afficher "température du 1er jour"
saisir temp
min, max ← temp
pour i de 2 à 365
   saisir temp
   si temp > max alors max ← temp
   si temp < min alors min ← temp
finpour
```

🎯 **Tâche :** Traduisez en Python. Attention à bien initialiser `min` et `max` avec la première valeur.

---

## 📈 Exercice 12 – Suite croissante ?

**Pseudo-code (version simple) :**

```
afficher "entrer une valeur"
saisir valeur
ancval ← valeur
croissant ← vrai
tantque valeur <> 0
   afficher "entrer une valeur"
   saisir valeur
   si valeur <= ancval et valeur <> 0 alors
      croissant ← faux
   finsi
   ancval ← valeur
fintantque
si croissant alors afficher "suite croissante"
sinon afficher "pas croissante"
```

🎯 **Tâche :** Reproduisez cette logique en Python.

---

## ♟️ Exercice 13 – Le jeu d’échecs et les grains de blé

**Pseudo-code :**

```
nbgrains ← 1
total ← 1
pour k de 2 à 64
   nbgrains ← nbgrains * 2
   total ← total + nbgrains
finpour
afficher total
```

🎯 **Tâche :** Traduisez cet algorithme en Python et affichez le total.

---

## 🔢 Exercice 14 – Nombre premier ?

**Pseudo-code :**

```
diviseur ← 2
tantque nombre mod diviseur <> 0 et diviseur < nombre
   diviseur ← diviseur + 1
fintantque
si diviseur = nombre alors
   afficher nombre, "est premier"
sinon
   afficher nombre, "n'est pas premier"
```

🎯 **Tâche :** Traduisez cet algorithme en Python. Utilisez l’opérateur `%` pour le modulo.

---

## 🎁 Exercice 15 (BONUS) – Mini‑labyrinthe textuel « Évadons‑nous ! »

**Objectif :** créer un petit jeu en mode texte où le joueur se déplace dans un labyrinthe jusqu’à la sortie en évitant les pièges et en gérant son énergie.

**Pseudo‑code (guide) :**

```
programme labyrinthe
  constantes
    LARGEUR, HAUTEUR
  variables
    grille : tableau 2D de caractères ('.'=vide, '#'=mur, 'S'=départ, 'E'=sortie, 'T'=piège)
    px, py : entiers (position joueur)
    energie : entier
    commande : chaîne

  procedure initialiser_grille()
    créer une grille de HAUTEUR lignes × LARGEUR colonnes remplie de '.'
    placer des murs '#' aléatoirement (densité raisonnable)
    placer quelques pièges 'T'
    placer 'S' en (px, py) et 'E' ailleurs
    // option avancée : garantir qu'un chemin existe (BFS/DFS)

  procedure afficher_grille()
    afficher la grille en remplaçant la case (px, py) par '@'
    afficher "Énergie : ", energie

  debut
    choisir LARGEUR, HAUTEUR (ex: 10×8), energie = 20
    initialiser_grille()
    repeter
      afficher_grille()
      afficher "Commande (Z/Q/S/D pour bouger, X pour quitter) :"
      saisir commande
      si commande ∈ {Z,Q,S,D} alors
        calculer (nx, ny) = nouvelle position
        si case (nx, ny) est un mur '#' alors
          afficher "Aïe, un mur !"
        sinon
          px, py ← nx, ny
          energie ← energie - 1
          si case (px, py) est un piège 'T' alors
            energie ← energie - 2
            afficher "Piège ! -2 énergie"
          finsi
        finsi
      finsi
    jusqu'à (case (px, py) est 'E') ou (energie ≤ 0) ou (commande = 'X')

    si case (px, py) est 'E' alors
      afficher "Bravo, évadé !"
    sinon si energie ≤ 0 alors
      afficher "Épuisé… Vous restez coincé."
    sinon
      afficher "Abandon."
    finsi
  fin
```

🎯 **Tâche :** traduire ce pseudo‑code en Python (sans librairie externe). Affichez la grille à chaque tour, l’avatar du joueur `@`, l’énergie restante, et gérez les collisions.

💡 **Indications si vous bloquez :**

* Représentez la grille par une **liste de listes** de caractères.
* Pour l’aléatoire : regardez le module `random` (`random.randint`).
* Pour éviter que la sortie soit bloquée, commencez par une **grille prédéfinie** (sans aléatoire), puis ajoutez l’aléatoire en bonus.
* Pour nettoyer l’écran entre deux affichages, vous pouvez simplement imprimer plusieurs lignes vides.
* Déplacements : `Z` (haut) = `py-1`, `S` (bas) = `py+1`, `Q` (gauche) = `px-1`, `D` (droite) = `px+1`.

🏆 **Défis optionnels (pour les plus rapides)**

* **Assurer un chemin** automatiquement (implémentez une recherche en largeur BFS).
* **Chronomètre** (comptez les tours) et **meilleur score** (énergie restante la plus haute).
* **Niveaux** : augmentez la taille, la densité de murs/pièges ou réduisez l’énergie.
* **Brouillard de guerre** : n’affichez que les cases autour du joueur.
* **Portes/Clés** : placez une clé `K` à récupérer avant d’atteindre `E`.

---

# 🏁 Bilan

Vous savez maintenant :

* exécuter un programme dans Thonny,
* traduire un pseudo-code en Python,
* utiliser les conditions et les boucles,
* écrire du code bien **indenté** et lisible.
* RDV en SLAM !
