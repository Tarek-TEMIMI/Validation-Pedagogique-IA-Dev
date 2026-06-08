# Programme — Pilotage du Développement par IA (méthodologie Tarek)

**Auteur :** Tarek — Consultant & Formateur Senior, Architecture IA & Automatisation
**Approche :** Méthodologie stack-agnostique de programmation assistée par IA, transposable sur n'importe quel langage/framework (.NET, TypeScript, Java, Python...)
**Format :** 5 jours (modulable 3-5 jours selon contexte)
**Stack outillage :** Claude Code, GitHub Copilot, ChatGPT, OpenRouter — agnostique vis-à-vis de la stack métier du client

---

## Philosophie

- **70% pratique / 30% théorie** : chaque concept suivi immédiatement d'un TP sur cas réel
- L'IA est un outil à **piloter**, pas une boîte magique : on enseigne autant les limites (hallucinations, doom loop, faux positifs) que les forces
- La méthodologie est **indépendante du langage** : ce qui compte, c'est le processus de pilotage (cadrage → génération → validation → intégration), pas la syntaxe
- Sécurité et bonnes pratiques injectées **dès le Jour 1**, pas en fin de parcours

---

## Jour 1 — Prompting professionnel & Cadrage

**Bloc 1 — Fondamentaux du prompting**
- Lexique IA générative appliqué au développement
- Structuration d'un prompt efficace en contexte d'équipe
- Patterns PRF (Prompt-Refine-Finalize) et IRF (Iterate-Refine-Finalize)
- Le **Doom Loop** : comment le repérer et en sortir

**Bloc 2 — Fichiers de cadrage**
- CLAUDE.md / copilot-instructions.md : structurer le contexte projet pour l'IA
- Warm-up sécurité : ce qu'on a le droit d'envoyer à un assistant IA (secrets, PII)

**TP** : Créer le fichier de cadrage du projet et observer son impact immédiat sur la qualité des réponses

---

## Jour 2 — Documentation & Génération de code

**Bloc 1 — Documentation comme contexte IA**
- Types de documentation utiles à un assistant IA
- Rédiger une doc technique exploitable comme source de vérité

**Bloc 2 — Génération encadrée**
- Injecter du code généré dans une base existante (monolithe/legacy)
- Respect des conventions internes via fichiers de cadrage
- Limites du "tout-automatique" en contexte industriel

**TP** : Documenter un module existant puis générer un composant conforme aux conventions, en s'appuyant sur cette doc comme contexte

---

## Jour 3 — Analyse, Compréhension & Refactoring

**Bloc 1 — Cartographie assistée**
- Cartographier les dépendances d'un module legacy via IA
- Expliquer une logique métier non documentée ou obfusquée

**Bloc 2 — Refactoring piloté**
- Utilisation de /fix et /optimize sur du code complexe
- Application des principes SOLID en contexte contraint
- Mesure d'impact : complexité cyclomatique avant/après

**TP** : Cartographier et refactorer un module du projet fil rouge, mesurer le gain

---

## Jour 4 — Debug, Tests & Validation critique

**Bloc 1 — Debug assisté**
- Diagnostic de runtime errors et stacktraces avec l'IA
- Interprétation des échecs de pipeline CI/CD et remédiation

**Bloc 2 — Tests pilotés par IA**
- TDD assisté : écrire les tests avant le code
- Génération de cas de test, edge cases, jeux de données
- *Frameworks alignés sur la stack du client* (ex. xUnit/NUnit/MSTest pour .NET, Jest pour TS, JUnit pour Java)
- Détection d'erreurs logiques et analyse critique du code généré (le réflexe "je ne valide jamais sans relire")

**TP** : Générer une suite de tests sur un module du fil rouge, viser une couverture cible, puis challenger chaque cas généré

---

## Jour 5 — Workflow Git, Sécurité & Projet de clôture

**Bloc 1 — Git & orchestration IA**
- Génération de messages de commit et de Pull Requests
- Résolution de conflits assistée, coordination d'équipe
- IDE assistants vs chat LLM vs outils CLI : quand utiliser quoi

**Bloc 2 — Sécurité (approfondissement)**
- Risques du code généré par IA, gestion des secrets et PII
- Vulnérabilités courantes et remédiation

**Bloc 3 — Projet fil rouge de clôture**
- Mini-projet bout-en-bout : spécification → génération → refactoring → tests → debug → PR
- Application de toutes les règles vues, dès la rédaction des prompts

**TP final** : Réalisation autonome encadrée, debrief collectif

---

## Ce qui distingue cette approche

1. **Transposabilité** : la méthode a été conçue et éprouvée sur plusieurs stacks (TypeScript, C#/.NET legacy, etc.) — le projet fil rouge "StockManager" en est un exemple concret
2. **Sécurité dès J1**, pas en fin de programme
3. **Mesure d'impact systématique** (complexité cyclomatique, couverture de tests) plutôt que du "ça a l'air de marcher"
4. **Esprit critique structuré** : chaque TP inclut une phase de validation/contestation du résultat IA, pas seulement de génération
