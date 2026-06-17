# EduBoard – Projet LaTeX PFE
**Rapport de Projet de Fin d'Études – ESPITA 2025/2026**  
**Auteure : Hayet BERRIRI**

---

## Structure du projet

```
pfe_latex/
├── main.tex                          ← Fichier principal (compiler celui-ci)
├── README.md
├── chapters/
│   ├── 00_acronymes_def.tex          ← Liste des abréviations
│   ├── 00_acronymes_manuel.tex       ← Guide d'usage des macros \ac{}
│   ├── 01_page_garde.tex             ← Page de garde (PDF inclus)
│   ├── 02_dedicaces.tex
│   ├── 03_remerciements.tex
│   ├── 05_introduction_generale.tex
│   ├── 06_chapitre1_presentation.tex ← Contexte, organisme, SCRUM
│   ├── 07_chapitre2_specifications.tex← Besoins fonctionnels/non fonctionnels
│   ├── 08_chapitre3_conception.tex   ← Architecture, UML, diagrammes
│   ├── 09_chapitre4_realisation.tex  ← Interfaces, tests
│   ├── 10_conclusion_generale.tex
│   ├── 11_bibliographie.tex
│   └── 12_annexes.tex                ← Code source, SQL, guide images
└── figures/
    ├── images/    ← Captures d'écran et logos (.png / .jpg)
    ├── diagrams/  ← Diagrammes UML exportés
    └── pdfs/      ← Page de garde PDF (page_de_garde (1).pdf)
```

---

## Compilation (Overleaf)

1. Créer un nouveau projet Overleaf.
2. Uploader **tous les fichiers** en respectant la structure ci-dessus.
3. Sélectionner `main.tex` comme fichier principal.
4. Compilateur : **pdfLaTeX**.
5. Compiler **deux fois** (table des matières, listes de figures/tableaux).

## Images à placer dans `figures/images/`

Voir `chapters/12_annexes.tex` → Annexe C pour la liste complète des fichiers
images attendus avec leur correspondance dans le rapport.

---

## Packages requis

| Package   | Usage                          |
|-----------|-------------------------------|
| acronym   | Gestion des abréviations       |
| booktabs  | Tableaux professionnels        |
| hyperref  | Liens cliquables               |
| pdfpages  | Inclusion de la page de garde PDF |
| subcaption| Sous-figures                  |
| minted    | Coloration syntaxique du code  |
| listings  | Code source alternatif         |
| tabularx  | Tableaux à largeur fixe        |

> **Note :** `minted` nécessite l'option `--shell-escape` (activée par défaut sur Overleaf).
