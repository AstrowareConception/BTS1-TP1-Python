# 🐍 TP 1 – Découverte de Python avec Thonny

## 🌟 Objectif du TP

Apprendre à écrire, exécuter et comprendre ses premiers programmes Python en traduisant des algorithmes simples.

---

## 🧮 1. Installation de l’environnement Thonny

### Étapes :

1. Rendez-vous sur : [https://thonny.org/](https://thonny.org/)
2. Cliquez sur **Download Thonny**.
3. Choisissez la version correspondant à votre système :

   * **Windows** → Thonny with Python included (recommandé)
   * **macOS** / **Linux** → version adaptée
4. Installez-le avec les options par défaut.
5. Lancez Thonny : vous verrez

   * une zone blanche (pour le code)
   * une zone en bas (la console Python)
   * un bouton **▶️** pour **exécuter** le programme.

---

## 🤓 2. Premiers pas avec Python

### ✨ Exemple minimal :

```python
print("Bonjour le monde !")
```

Appuyez sur **▶️** pour exécuter le code.

---

## 🔧 3. Les bases du langage Python

### 🔢 Les variables

Une variable sert à **stocker une valeur**.

```python
nom = "Alice"
age = 20
```

### 🔍 L'affichage

```python
print("Bonjour", nom)
```

### ⌨️ La saisie au clavier

```python
nom = input("Entrez votre nom : ")
print("Bonjour", nom)
```

> Par défaut, `input()` renvoie du texte (une *chaîne de caractères*).
> Pour des nombres, on convertit : `int(input(...))` ou `float(input(...))`.

### ⚙️ Les conditions

```python
if condition:
    # bloc d'instructions
elif autre_condition:
    # autre bloc
else:
    # dernier cas
```

> **Important :** L'indentation (les espaces au début de la ligne) indique les blocs.
> En Python, **4 espaces** = 1 niveau d'indentation.
> Pas d'accolades, pas de "finsi" ! L'indentation *fait partie du code*.

Exemple :

```python
if age >= 18:
    print("Majeur")
else:
    print("Mineur")
```

### 🔄 Les boucles

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

Chaque exercice = un fichier Python :

* `exo01.py`
* `exo02.py`
* ...

Sauvegardez avant d'exécuter !

---

# 🔮 Partie 2 – Les exercices Python 

Chaque exercice est à écrire dans un fichier différent. Des indices sont donnés.

---

## 🤔 Exercice 1 – Trace d’un programme

**But :** écrire un programme avec des conditions et des calculs simples.

Demandez à l'utilisateur de saisir A, B, C.
Traduisez ensuite la séquence logique du TD (avec `if`, `and`, `or`, etc.).
Affichez la valeur finale de A, B et C.

*Indice :* les opérateurs sont `==`, `!=`, `<`, `>`, `and`, `or`.

---

## 👤 Exercice 2 – Bonjour Madame / Monsieur

Demandez le **nom** et le **sexe (F/M)**.
Tant que la saisie n'est pas correcte, reposez la question.

*Indice :* utilisez une boucle `while` avec `not in ["F", "M"]` et `upper()` pour uniformiser les lettres.

---

## 🤖 Exercice 3 – Logique conditionnelle

Traduisez en expressions Python les conditions suivantes :

1. X, Y, Z sont identiques
2. X, Y, Z sont identiques mais différents de T
3. X est entre Y et T
4. Parmi X, Y, Z, deux valeurs seulement sont identiques

*Indice :* testez vos expressions avec des valeurs différentes et `print()`.

---

## 🏢 Exercice 4 – Une ville et ses habitants

Demandez le nom d'une ville et son nombre d'habitants.
Affichez : *NomVille possède X habitants.*

---

## 💶 Exercice 5 – Conversion Euro / Franc

Demandez un prix en Euro et affichez sa valeur en Franc (1€ = 6,55957 F).

*Indice :* utilisez une variable pour stocker le taux.

---

## 📊 Exercice 6 – Moyenne et message

Demandez une moyenne et affichez :

* Passage si moyenne ≥ 10
* Redoublement si moyenne ≥ 8
* Exclusion sinon

*Indice :* en Python, les `if` peuvent être imbriqués.

---

## 🚓 Exercice 7 – Feu tricolore du robot

Demandez la couleur d'un feu (rouge/orange/vert).
Répétez la question tant que la saisie n'est pas valide.
Affichez l'action du robot : s'arrêter / ralentir / passer.

---

## 📈 Exercice 8 – Moyenne de plusieurs notes

Saisissez plusieurs notes (au moins une).
Après chaque note, demandez si l'utilisateur veut continuer (O/N).
Affichez la moyenne finale.

---

## ➕ Exercice 9 – Compter positifs et négatifs

Demandez 20 nombres et comptez combien sont positifs (ou nuls) et combien sont négatifs.

*Indice :* utilisez une boucle `for` et un compteur.

---

## 📊 Exercice 10 – Note min et max

Saisissez 30 notes et affichez la plus basse et la plus haute.

*Indice :* initialisez `min_note` et `max_note` avant la boucle.

---

## 🌡️ Exercice 11 – Températures de l’année

Saisissez 365 températures.
Affichez la température la plus basse et la plus haute.

*Indice :* commencez avec la première température comme base.

---

## 📊 Exercice 12 – Suite croissante ?

Saisissez des valeurs jusqu'à entrer 0.
Affichez si la suite est strictement croissante.

*Indice :* comparez chaque valeur avec la précédente.

---

## ♟️ Exercice 13 – Le jeu d'échecs et les grains de blé

Calculez combien de grains de blé sont posés sur un échiquier si on double à chaque case.

*Indice :* utilisez une boucle `for` et une variable `total`.

---

## 🔢 Exercice 14 – Nombre premier ?

Demandez un nombre et affichez s'il est premier ou non.

*Indice :* testez la divisibilité avec `%` et une boucle `while`.

---

# 🚀 Bilan

Vous savez maintenant :

* exécuter un programme dans Thonny,
* utiliser les entrées/sorties,
* manipuler les conditions et les boucles,
* organiser votre code proprement avec l'indentation.

✨ Bravo, vous venez d'entrer dans le monde de la programmation Python !
