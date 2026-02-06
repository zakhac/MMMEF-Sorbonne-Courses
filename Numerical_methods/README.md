# Numerical Methods for Optimization - Cours LaTeX

Ce projet contient les sources LaTeX pour le cours complet de Méthodes Numériques en Optimisation.

## Structure du Projet

*   **`NumericalMethods.tex`** : Fichier maître (anciennement `main.tex`). Définit le préambule, les packages, le style (`tcolorbox`), et inclut tous les chapitres. Compilez ce fichier pour générer le PDF final.
*   **`chapitreX.tex`** : Fichiers sources pour chaque chapitre individuel.
    *   `chapitre1.tex` : Introduction
    *   `chapitre2.tex` : Optimisation sans contraintes (théorie)
    *   `chapitre3.tex` : Gradient conjugué
    *   ...
    *   `chapitre12.tex` : Méthodes de pénalité (dernier chapitre)
*   **`references.bib`** : Fichier bibliographique BibTeX contenant toutes les références du cours (Nocedal, Wright, etc.).
*   **`images/`** : Dossier contenant les figures et illustrations (PNG, PDF, etc.).
*   **`Makefile`** : Script pour automatiser la compilation.

## Compilation

Pour générer le document complet `NumericalMethods.pdf` avec la bibliographie à jour :

1.  **Avec Make** (Recommandé) :
    ```bash
    make
    ```

2.  **Manuellement** :
    ```bash
    pdflatex NumericalMethods.tex
    bibtex NumericalMethods
    pdflatex NumericalMethods.tex
    pdflatex NumericalMethods.tex
    ```

## Conventions

*   **Algorithmes** : Les algorithmes sont formatés avec le package `algorithm2e` et le style personnalisé défini dans le préambule (mots-clés en bleu, commentaires en vert).
*   **Théorèmes/Définitions** : Utilisent `tcolorbox` pour des encadrés colorés (Rouge=Théorème, Bleu=Définition, Orange=Proposition, Violet=Lemme).
*   **Citations** : Utiliser `\cite{cle_bibtex}` pour référencer un ouvrage de `references.bib`.

## État des Chapitres

*   **Chapitres 1-8** : Contenu complet, algorithmes en anglais (comme fourni par le professeur) ou français selon le contexte initial.
*   **Chapitres 9-12** : Contenu théorique et algorithmes (Conditions d'optimalité, Simplexe, NON-linéaire, Pénalité) intégrés. En cours de révision et normalisation.
