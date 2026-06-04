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
