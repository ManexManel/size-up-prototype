# Handoff — test reference-match-loop (28/09/2026)

## Fait
- `index.html` v3 : marque fictive DÉMO TEST (cuisiniste), palette MNX (crème / #0C0B1D / jade #00A86B). Référence (Buttermax) : mécanique seule, marque non reprise.
- Boucle : 3 itérations sur 5 (`versions/index.v1..v3.html`). v1 violait GATE 0 (jaune/noir/nom de la réf), corrigé en v2.
- Preuve : `preuve/M1..M5_ref_vs_rendu.png` (réf | desktop 1440 | mobile 375). Console vide, pas de débordement horizontal.
- `spec.md` (fournie par Manel) copiée à la racine.
- PR draft : ManexManel/size-up-prototype#1, Vercel preview OK.

## Écarts restants (assumés, niveau 1 sans asset)
- Objet hero = disque acier CSS, pas un appareil 3D volumétrique.
- Grille (hotte/four/plaque) et main du M5 en CSS ; encre du M5 approximée (bord animé) ; glitch RGB M2 en CSS.
- Non testé : poids exact, repli sans WebGL, 60 FPS mesurés.

## Statut
Auto-vérifié, NON audité (pas d'auditeur indépendant).

## Prochaine étape (décision Manel)
- Hero en Three.js + GLB : passe par `assets-3d-pipeline` ; toute dépense Meshy = OK Manel d'abord.
- Audit indépendant si demandé (sous-agent cherchant à REJETER sur les captures).
- Loi §2 : ce test est de la MACHINE, à ne pousser qu'après le socle du jour.

## Fichiers touchés
index.html, spec.md, versions/, preuve/, systemes/handoff.md
