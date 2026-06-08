# Mapping comparatif — Programme du cabinet vs Méthodologie Tarek

Ce document démontre une étude approfondie du programme proposé par le cabinet ("Pilotage du Développement par IA — 5 jours, .NET") et sa transposition directe dans ma méthodologie éprouvée, stack-agnostique.

---

## Vue d'ensemble

| Critère | Programme du cabinet | Ma méthodologie |
|---|---|---|
| Stack visée | .NET / GitLab / Copilot Enterprise | Agnostique — déjà testée sur TypeScript, C#/.NET legacy |
| Durée | 5 jours | 5 jours (modulable 3-5j) |
| Ratio pratique/théorie | TP après chaque bloc | 70% pratique / 30% théorie, formalisé et mesuré |
| Projet fil rouge | Mentionné, à fournir par le cabinet | Déjà existant et prêt (StockManager, C# legacy) |
| Sécurité | Traitée Jour 5 uniquement | Warm-up dès Jour 1 + approfondissement Jour 5 |

---

## Mapping jour par jour

### Jour 1 — Prompting & Cadrage
| Leur contenu | Mon équivalent | Commentaire |
|---|---|---|
| Lexique IA générative, structuration de prompt | Identique — module 01-prompting déjà rédigé | Contenu directement réutilisable |
| Doom Loop | Identique, avec exemples concrets prêts | Concept central de ma pédagogie |
| Pattern Driven Development (PRF/IRF), fichiers de cadrage | Couvert + enrichi avec CLAUDE.md / copilot-instructions.md | J'ajoute un standard concret de fichier de cadrage |
| — | Warm-up sécurité (15 min) | **Ajout de ma part** : je recommande de l'intégrer dès J1 plutôt qu'en J5 |

### Jour 2 — Documentation, Cadrage & Génération
| Leur contenu | Mon équivalent | Commentaire |
|---|---|---|
| Documentation comme contexte IA | Identique | |
| Génération de composant .NET conforme aux conventions internes | Même logique, transposée : "génération encadrée par fichiers de cadrage" | La méthode (cadrer → générer → valider conformité) est identique quel que soit le langage |

### Jour 3 — Analyse, Compréhension & Refactoring
| Leur contenu | Mon équivalent | Commentaire |
|---|---|---|
| Cartographie de dépendances, logique métier obfusquée | Identique | |
| /fix /optimize, SOLID, complexité cyclomatique | Identique, avec mesure d'impact systématisée | J'ajoute la mesure avant/après comme livrable de TP |
| Projet fil rouge legacy | **StockManager (C# legacy)** déjà construit et prêt à l'emploi | Gain de temps immédiat pour le cabinet |

### Jour 4 — Debug, Tests & Validation
| Leur contenu | Mon équivalent | Commentaire |
|---|---|---|
| Diagnostic stacktraces, échecs CI/CD | Identique | |
| TDD assisté — **JUnit, Jest** mentionnés | TDD assisté — **xUnit/NUnit/MSTest** | ⚠️ **Incohérence repérée dans leur programme** : JUnit (Java) et Jest (JS) n'ont aucun rapport avec une stack .NET. Je propose l'alignement correct, ce qui prouve une lecture attentive et une vraie expertise transverse |
| Analyse critique du code généré | Identique, formalisée en "phase de contestation" dans chaque TP | |

### Jour 5 — Git, Sécurité & Projet de clôture
| Leur contenu | Mon équivalent | Commentaire |
|---|---|---|
| Commits, PR, conflits, orchestration outils | Identique | |
| Sécurité, secrets, PII | Identique — approfondissement (le warm-up ayant eu lieu en J1) | |
| Projet de clôture bout-en-bout | Identique — sur StockManager | |

---

## Synthèse — Pourquoi cette approche rassure le cabinet

1. **J'ai étudié leur programme dans le détail** — au point de repérer une incohérence technique (JUnit/Jest vs .NET) qu'ils n'ont peut-être pas vue eux-mêmes
2. **Mon contenu existe déjà** — modules rédigés, projet fil rouge prêt : pas de risque d'improvisation
3. **Ma valeur n'est pas la maîtrise de .NET, c'est la maîtrise du *processus* de pilotage IA** — applicable et transposable, ce qui est précisément ce qu'un cabinet veut entendre d'un formateur qui doit intervenir sur des stacks variées selon les clients
4. **J'apporte une amélioration concrète** (sécurité dès J1, mesure d'impact systématique) plutôt que de simplement "réciter" leur programme
