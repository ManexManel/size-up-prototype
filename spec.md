# Spec — test reference-match-loop (28/09/2026)

Référence : enregistrement `Enregistrement 2026-09-27 123723.mp4` (26 s, scroll d'un site studio). Frames : `frames/sheet_1..4.png`.
**Test, pas un prospect.** Marque fictive « DÉMO TEST », niche cuisiniste (niche en test, voir mémoire), palette MNX (crème / encre #0C0B1D / jade #00A86B).
On transpose la MÉCANIQUE, jamais la marque de la référence (nom, texte, jaune/noir, objets dorés : non repris).

## Moments (frame de référence → comportement)
| M | Frame réf | Apparence | Comportement (verbes) |
|---|---|---|---|
| M1 | sheet_1 #1-2, sheet_4 #1 (0:02, 0:04, 0:00) | fond uni clair, énorme titre noir, objet 3D métallique flottant au centre-droit, sous-titre en petites capitales | **une encre noire liquide suit le curseur** et laisse une traînée qui s'épaissit puis s'efface (gooey) ; l'objet flotte, tourne lentement, s'incline vers le curseur |
| M2 | sheet_1 #2-3 (0:04-0:06) | bande sombre pleine largeur, effet glitch avec séparation RGB, bords irréguliers | apparaît au scroll entre le hero et le texte ; défile en parallaxe ; frémit |
| M3 | sheet_1 #3, sheet_2 #1-2 (0:06-0:12) | paragraphe manifeste en très gros capitales serrées, « WHO WE ARE » en micro-label | **sous l'encre, le texte s'inverse (blanc sur noir)** ; le texte reste lisible partout |
| M4 | sheet_1 #4, sheet_2 #3-4 (0:08-0:16) | grille 3 colonnes fines, un objet 3D métallique par cellule, micro-labels (client + année) | l'objet tourne au survol ; **une tache de couleur flat s'ouvre derrière** (vert, rouge, orange) et suit ; cellule voisine ne bouge pas |
| M5 | sheet_3 #1-3 (0:18-0:22) | section noire plein écran, gros « REACH OUT » jaune, email, pastilles de réseaux, objet 3D (main) au centre | l'encre noire remonte depuis la section précédente (bord ondulé qui bouge) ; objet flotte devant le titre |

## Critères vérifiables
- M1 : encre visible derrière le titre, objet 3D à ≥ 25 % de la hauteur de vue, aucun élément coupé à 1440 et 375.
- M3 : texte blanc sur l'encre, sombre ailleurs, contraste lisible.
- M4 : 3 objets alignés sur les 3 cellules, tache visible au survol.
- M5 : bouton d'action (réserver 10 minutes) atteignable sur mobile.
- Repli : `prefers-reduced-motion` / pas de WebGL → page lisible, action de contact intacte.
- Poids `index.html` < 2 Mo, console vide.

## Écarts connus dès la spec (à surveiller)
- Objets procéduraux (niveau 1, aucun asset) : la finesse des modèles de la référence ne sera pas atteinte. Écart assumé.
- Glitch RGB du M2 approximé en CSS.
