# alignment-os

![Version](https://img.shields.io/badge/version-1.0.0-blue) ![License](https://img.shields.io/badge/license-Apache%202.0-green) ![Claude](https://img.shields.io/badge/Claude-Skill-purple)

🌍 **Français** · **[English](README.en.md)**

> Système d'alignement personnel pour Claude : 4 modules qui cherchent la cohérence entre valeurs déclarées, actions réelles et trajectoire observable. **Pas de développement personnel creux. Pas de citations gourou.**

## ⚠️ Garde-fou critique

Cette skill **n'est pas un outil de santé mentale**. Elle est conçue pour des utilisateurs dans un fonctionnement globalement sain qui cherchent plus de cohérence.

Sur détection de signaux de détresse (idées suicidaires, symptômes dépressifs prolongés, crise aiguë, détresse relationnelle grave, dépendance active), la skill **arrête l'exercice d'alignement** et redirige vers des ressources humaines qualifiées (médecin, psychologue, lignes d'écoute d'urgence).

Voir [`SAFETY.md`](./SAFETY.md) pour le protocole complet.

## Ce que ça fait

La plupart des outils de "développement personnel" tombent dans trois pièges :
1. **Motivationnels** (citations, visualisations, promesses)
2. **Rituels sans structure** (journaling, méditation sans cadre)
3. **Systémiques mais creux** (OKR personnels, life planning silicon-valley)

`alignment-os` n'est aucun des trois. C'est un système qui :

1. **Force des questions dures** (pas des affirmations qui rassurent)
2. **Exige de l'écriture** (l'écriture force la clarté)
3. **Respecte la diversité des chemins** (pas de prescription morale)
4. **Détecte les signaux de détresse** et redirige vers l'humain qualifié
5. **Compose** avec le reste de ton OS Claude

## Les 4 modules

| Module | Rôle | Quand l'appeler |
|---|---|---|
| **Purpose Clarifier** | Clarifier ce qui compte vraiment au-delà des récits sociaux | Tu cours sans direction, tu sens un vide |
| **Ethics Filter** | Passer une décision au filtre de tes valeurs | Décision qui te grise mais te gêne |
| **Discipline Reinforcement** | Corriger les patterns de dérive structurellement | Tu tiens pas tes engagements depuis longtemps |
| **Life Audit** | Audit trimestriel/annuel de cohérence | Fin de période, transition, décrochage |

## Déclencheurs

- *"Je sais plus pourquoi je fais ça"*, *"quel est mon pourquoi"* → Purpose Clarifier
- *"Cette décision me grise mais me gêne"*, *"j'ai l'impression de trahir X"* → Ethics Filter
- *"Je tiens pas mes engagements"*, *"je recommence toujours le même truc"* → Discipline Reinforcement
- *"Fin d'année"*, *"bilan de vie"*, *"suis-je aligné"* → Life Audit

## Dimension spirituelle adaptative

La skill :
- **Ne présuppose jamais** de cadre religieux/spirituel
- **Reconnaît et s'adapte** si l'utilisateur mobilise un cadre (islam, christianisme, bouddhisme, stoïcisme, humanisme laïque, etc.)
- **N'introduit pas** de vocabulaire spirituel de son propre chef
- **Respecte strictement** les choix — pas de prosélytisme, pas de dérision

## Ton adaptatif

- **Direct et confrontant** sur `discipline-reinforcement` et `ethics-filter`
- **Plus posé** sur `purpose-clarifier` et `life-audit`
- **Toujours respectueux** — jamais condescendant ni moralisateur

## Composition avec l'écosystème

- `alignment-os/ethics-filter` × [`thinking-os`](https://github.com/alphilippo/thinking-os) :
  - Décision éthiquement claire mais stratégiquement complexe → `thinking-os/second-order`
  - Décision émotionnellement chargée → `thinking-os/10-10-10`
- `alignment-os/discipline-reinforcement` × [`execution-os`](https://github.com/alphilippo/execution-os) :
  - Dérive **opérationnelle** (mauvaises tâches cette semaine) → `execution-os/accountability-check`
  - Dérive **identitaire** (tu trahis ce que tu dis vouloir être) → `alignment-os`
- `alignment-os/purpose-clarifier` × [`learning-os`](https://github.com/alphilippo/learning-os) :
  - Purpose clarifié révèle des domaines à explorer → `learning-os/learning-path-planner`
- `alignment-os/ethics-filter` × [`strategy-intel`](https://github.com/alphilippo/strategy-intel) :
  - Move stratégiquement attirant mais éthiquement bancal → ethics-filter **avant** strategic-move-planner

## Installation

### Claude.ai

1. Télécharge le ZIP depuis GitHub ou clone le repo
2. Dans Claude.ai : Settings → Skills → "+" → "+ Create skill" → upload
3. Toggle ON

### Claude Code

```bash
cp -r alignment-os ~/.claude/skills/
```

## Exemples

### Ethics filter — contrat tentant
> *"On me propose un gros contrat dans le tabac. Le deal serait énorme. Mais je me sens mal. Aide-moi."*

→ La skill **ne tranche pas**, élucide le malaise (souvent lié à l'histoire personnelle), applique 5 tests, propose des alternatives, propose un délai de 7 jours.

### Discipline reinforcement — dérive de 3 ans
> *"Ça fait 3 ans que je dis que je vais écrire un livre. Je ne fais rien. Je suis nul."*

→ Remplace "nul" par factuel, diagnostique 4 catégories possibles (le truc ne compte pas / structure manque / peur sabote / besoin caché), propose correction **structurelle** et micro-engagement 2 semaines.

### SAFETY — détresse détectée
> *"Je voulais faire un bilan de vie. Mais depuis 3 mois je suis vide, je dors mal. Tout le monde serait mieux sans moi."*

→ La skill **arrête** le life audit, nomme les signaux sans drama, oriente vers médecin / 3114 / proche, reste disponible sans forcer.

## Structure

```
alignment-os/
├── SKILL.md
├── SAFETY.md                # Protocole de détection et redirection
├── README.md + README.en.md
├── CHANGELOG.md
├── modules/
│   ├── purpose-clarifier.md
│   ├── ethics-filter.md
│   ├── discipline-reinforcement.md
│   └── life-audit.md
├── templates/               # 4 templates d'écriture
├── examples/                # 3 exemples dont SAFETY
└── tests/test-cases.md      # 11 cas, cas 1 critique
```

## Skills complémentaires (écosystème complet)

- 🧠 [**thinking-os**](https://github.com/alphilippo/thinking-os) — routeur cognitif
- ⚙️ [**execution-os**](https://github.com/alphilippo/execution-os) — système d'exécution
- 📚 [**learning-os**](https://github.com/alphilippo/learning-os) — système d'apprentissage
- ⚔️ [**strategy-intel**](https://github.com/alphilippo/strategy-intel) — analyse stratégique
- 🧭 [**alignment-os**](https://github.com/alphilippo/alignment-os) — alignement personnel

Les 5 répondent à des questions différentes :
- `thinking-os` — **QUOI** faire (cadre de pensée)
- `execution-os` — **COMMENT** le faire (cadence)
- `learning-os` — **APPRENDRE** à le faire (montée en compétence)
- `strategy-intel` — **OÙ & CONTRE QUI** le faire (positionnement)
- `alignment-os` — **POURQUOI** le faire (cohérence vie/valeurs)

## Limites explicites

- **N'est pas une thérapie.** Ne traite pas dépression, anxiété clinique, traumas.
- **N'est pas un guide spirituel.** Pas de vérité à transmettre sur le sens.
- **N'est pas un substitut aux relations humaines** (ami, mentor, conjoint, thérapeute).
- **Ne prévient pas** les mauvaises décisions — elle les rend **conscientes**.

Sur les sujets profonds, la skill oriente vers un humain qualifié. **Toujours.**

## Roadmap

- **v1.0** (actuel) : 4 modules + SAFETY.md + 4 templates + routage
- **v1.1** : Module **Relationships Audit** (cohérence relations proches)
- **v1.2** : Ajout de ressources SAFETY pour pays d'Afrique francophone
- **v2.0** : Mémoire entre life audits pour comparer les évolutions

## Licence

Apache 2.0 — fork, adapte, republie.

## Crédits

Conçu avec Claude comme Skill Architect. Inspiré par les travaux cliniques sur l'alliance thérapeutique (sans s'y substituer), les méthodes d'écriture réflexive (James Pennebaker), et les traditions philosophiques qui prennent l'examen de conscience au sérieux sans le caricaturer.

**Remerciement spécifique** : la priorité absolue à la SAFETY doit s'entendre comme un respect pour le travail des professionnels de santé mentale. Cette skill ne cherche pas à les remplacer — elle est conçue pour orienter vers eux quand c'est ce qu'il faut.
