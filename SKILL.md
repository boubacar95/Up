# resume-diagnoser

Analyse un CV (PDF ou texte) et retourne un rapport de diagnostic structuré.

## Utilisation

```
/resume-diagnoser [chemin-vers-le-cv]
```

## Ce que fait le skill

1. Lit le fichier CV fourni par l'utilisateur
2. Identifie les points forts, les faiblesses et les sections manquantes
3. Vérifie la mise en forme, la densité des mots-clés et la compatibilité ATS
4. Retourne une liste priorisée d'améliorations

## Format de sortie

- **Score** : note globale du CV (0–100)
- **Points forts** : ce qui fonctionne bien
- **Faiblesses** : ce qui doit être amélioré
- **Sections manquantes** : sections attendues mais absentes
- **Problèmes ATS** : mots-clés ou mise en forme pouvant nuire au tri automatique
- **Actions à entreprendre** : liste classée de corrections concrètes

## Critères d'analyse

- **Clarté** : le CV est-il lisible et bien structuré ?
- **Pertinence** : les expériences correspondent-elles au poste visé ?
- **Quantification** : les réalisations sont-elles chiffrées ?
- **Longueur** : le CV respecte-t-il la norme (1 à 2 pages) ?
- **Orthographe** : absence de fautes de grammaire et d'orthographe
- **Mots-clés** : présence de termes recherchés par les recruteurs

## Exemple de rapport

```
Score : 72/100

Points forts :
  - Expériences bien détaillées
  - Mise en forme propre et lisible

Faiblesses :
  - Pas de chiffres pour quantifier les réalisations
  - Résumé professionnel absent

Sections manquantes :
  - Profil / Résumé
  - Compétences techniques

Problèmes ATS :
  - Utilisation d'un tableau (non lisible par certains ATS)
  - Manque de mots-clés liés au domaine

Actions à entreprendre :
  1. Ajouter un résumé professionnel en haut du CV
  2. Quantifier chaque réalisation (ex: "augmenté les ventes de 20%")
  3. Remplacer le tableau par une liste simple
  4. Intégrer des mots-clés du secteur ciblé
```

## Notes

- Fonctionne avec les formats PDF, DOCX et texte brut
- Peut être combiné avec `/resume-recruiter` pour un retour côté recruteur
