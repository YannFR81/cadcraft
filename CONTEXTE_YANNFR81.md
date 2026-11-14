# Contexte du fork YannFR81 — CADCraft

> Le fichier `AGENTS.md` de ce dépôt est celui du projet d'origine (storytold/cadcraft) : **il s'applique et
> ne doit pas être modifié.** Ce fichier-ci ajoute seulement le contexte propre au fork.

Amont : storytold/cadcraft (clone open source d'AutoCAD en Rust).

## Le projet côté YannFR81
- Traduction française / harmonisation terminologique : **branche `i18n-fr-harmonize`** (PR ouverte vers l'amont).
- Tests d'allers-retours DWG/DXF entre CADCraft et AutoCAD 2027.
- `main` suit l'amont.

## Règles communes à tous les agents (Claude, Gemini / Antigravity, autres)

- **Propriétaire du fork :** YannFR81, projeteur routier (conception routière, AutoCAD / COVADIS).
  C'est lui qui tranche les choix métier et de terminologie.
- **Crédit :** uniquement sous le pseudo **YannFR81**, jamais de nom réel (commits, README, feuilles de route, PR).
- **Langue :** français pour la documentation, les messages de commit et les échanges ; apostrophe typographique ’ dans les textes d'interface.
- **Relations avec le dépôt d'origine (amont) :** proposer d'abord par une *issue* ; n'ouvrir une PR qu'après
  réponse des mainteneurs. Ne jamais pousser ni ouvrir de PR vers l'amont sans accord explicite de YannFR81.
- **Fichiers propres au fork :** `CONTEXTE_YANNFR81.md` et `NOTES_REVUE.md`
  ne doivent **jamais** figurer dans une branche proposée à l'amont. Créer les branches destinées à l'amont
  à partir de la branche de l'amont (`upstream/<branche>`), ou retirer ces fichiers avant la PR.
- **Pas de force-push** sur une branche dont une PR est ouverte.

## Travail en binôme

1. Un agent écrit, **l'autre relit** : aucun agent ne valide seul son propre travail.
2. Calculs normatifs ou moteur de calcul : écrire ou compléter d'abord les **tests sur cas de référence**
   (guides, abaques, exemples publiés), puis modifier le code. Un résultat de référence qui change = arrêt et signalement.
3. À la fin de chaque session, ajouter une entrée en tête de `NOTES_REVUE.md`
   (date, agent, branche, fait / vérifié / en suspens / question pour YannFR81).
4. Avant de commencer, lire `NOTES_REVUE.md` pour reprendre là où l'autre agent s'est arrêté.
