# Projet AMS – Algorithmique Avancée et Programmation (Graphes)

## Objectif

Ce projet consiste à modéliser et analyser un réseau routier sous forme de graphe. Il permet de manipuler des sommets (noeuds) et des arcs représentant des intersections et des routes. Plusieurs algorithmes de parcours et de traitement y sont intégrés, notamment :

- Création d’un graphe orienté pondéré à partir de fichiers `.csv`
- Construction de la liste d’incidence
- Calcul des degrés des noeuds
- Recherche de chemin entre deux noeuds (DFS)
- Recherche du plus court chemin (BFS)
- Recherche d’itinéraire par nom de rue

## Arborescence

.
├── include/         -> Fichiers d'en-tête (.h)
├── src/             -> Fichiers source (.cpp)
├── arcs.csv         -> Fichier contenant les arcs du graphe
├── nodes.csv        -> Fichier contenant les noeuds du graphe
├── Makefile         -> Fichier de compilation
└── README.md        -> Ce fichier

## Compilation et exécution

Depuis la racine du projet :

### Compilation

make

### Exécution

./bin/main

## Fonctionnalités principales

| Fonction                            | Description                                                                 |
|-------------------------------------|-----------------------------------------------------------------------------|
| `g.afficher()`                      | Affiche les noeuds et le nombre d'arcs du graphe                           |
| `g.degre(n)`                        | Affiche les `n` noeuds ayant le plus grand degré                           |
| `g.chemin("id1", "id2")`            | Affiche un chemin entre deux noeuds avec un parcours en profondeur (DFS)   |
| `g.plusCourtChemin("id1", "id2")`   | Affiche le plus court chemin (en nombre d’arcs) via un parcours en largeur (BFS) |
| `g.itineraire("rue1", "rue2")`      | Recherche un itinéraire entre deux rues par leur nom (version utilisateur ou test) |

## Auteur

- Nom : Yanis Laftimi  
- Filière : L2 Informatique – Groupe 4  
- Année : 2024-2025
