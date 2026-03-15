# PROCESS GESTION DE PROJET — Guide complet
> Basé sur PMBOK, PRINCE2, Agile, OKR et meilleures pratiques PM
> Version 1.0 — 2026-03-13

---

## SOMMAIRE

1. [Phase 1 — Initialisation du projet](#1-initialisation)
2. [Phase 2 — Planification](#2-planification)
3. [Phase 3 — Exécution quotidienne](#3-exécution-quotidienne)
4. [Phase 4 — Animation de réunions](#4-animation-de-réunions)
5. [Phase 5 — Communication & Parties prenantes](#5-communication--parties-prenantes)
6. [Phase 6 — Suivi — Gantt / KPI / Reporting](#6-suivi--gantt--kpi--reporting)
7. [Phase 7 — Clôture du projet](#7-clôture-du-projet)
8. [Outils & Templates de référence](#8-outils--templates)

---

## 1. INITIALISATION

### 1.1 Déclenchement — Les premières questions à poser

Avant de créer quoi que ce soit, répondre à ces 5 questions :

```
1. POURQUOI ce projet existe-t-il ? (problème ou opportunité)
2. QU'EST-CE QU'ON DOIT LIVRER exactement ? (périmètre)
3. POUR QUI ? (bénéficiaires, commanditaires)
4. AVANT QUAND ? (contrainte de délai)
5. AVEC QUOI ? (budget, ressources disponibles)
```

> **Technique : Le Problem Statement**
> Compléter cette phrase avant de démarrer :
> *"Actuellement [situation], ce qui provoque [impact négatif].
> Ce projet vise à [objectif], afin que [bénéfice attendu],
> mesuré par [indicateur de succès]."*

---

### 1.2 Charte de projet (Project Charter)

Document fondateur — à faire valider par le commanditaire.

```markdown
## CHARTE DE PROJET

Nom du projet :
Date de création :
Chef de projet :
Commanditaire :

### Objectif (SMART)
- Spécifique :
- Mesurable :
- Atteignable :
- Réaliste :
- Temporel :

### Périmètre
IN SCOPE (ce qu'on fait) :
- ...

OUT OF SCOPE (ce qu'on ne fait PAS) :
- ...

### Livrables principaux
1.
2.
3.

### Contraintes
- Budget :
- Délai :
- Ressources :
- Contraintes techniques :

### Hypothèses
- ...

### Risques identifiés à date
- ...

### Parties prenantes clés
| Nom | Rôle | Intérêt | Influence |
|-----|------|---------|-----------|

### Critères de succès
- ...

### Approbation
Commanditaire : _____________ Date : _______
Chef de projet : _____________ Date : _______
```

---

### 1.3 Identification des parties prenantes

> **Technique : Matrice Pouvoir / Intérêt (Power/Interest Grid)**

```
                    INTÉRÊT
                Faible      Fort
POUVOIR  Fort | SATISFAIRE | GÉRER ACTIVEMENT |
         Faible| SURVEILLER | TENIR INFORMÉ   |
```

- **Gérer activement** → communication régulière, implication forte
- **Satisfaire** → tenir au courant des décisions clés
- **Tenir informé** → newsletters, comptes-rendus
- **Surveiller** → veille légère

---

### 1.4 Kick-off meeting — Checklist

```
Avant le kick-off :
- [ ] Charte de projet validée par le commanditaire
- [ ] Liste des parties prenantes finalisée
- [ ] Ordre du jour envoyé 48h avant
- [ ] Salle / lien Teams réservé
- [ ] Supports préparés

Pendant le kick-off :
- [ ] Présenter le contexte et les enjeux (POURQUOI)
- [ ] Présenter les objectifs et livrables (QUOI)
- [ ] Clarifier les rôles et responsabilités (QUI)
- [ ] Présenter le planning macro (QUAND)
- [ ] Ouvrir sur les questions / risques
- [ ] Valider les prochaines étapes

Après le kick-off :
- [ ] Compte-rendu envoyé sous 24h
- [ ] Actions identifiées assignées
- [ ] Note index projet créée dans OneNote
```

---

## 2. PLANIFICATION

### 2.1 Décomposition du travail — WBS

> **Work Breakdown Structure** : décomposer le projet en livrables,
> puis en lots de travail, puis en tâches.

```
Projet
├── Livrable 1
│   ├── Lot de travail 1.1
│   │   ├── Tâche 1.1.1
│   │   └── Tâche 1.1.2
│   └── Lot de travail 1.2
├── Livrable 2
│   └── ...
└── Livrable 3
    └── ...
```

**Règle des 8/80** : une tâche ne doit pas durer moins de 8h
ni plus de 80h. Au-delà, la décomposer.

---

### 2.2 Estimation des charges

> **Technique : Planning Poker (Agile)**
> Chaque membre de l'équipe estime indépendamment,
> puis on discute les écarts. Évite l'effet de conformité.

> **Technique : Estimation par analogie**
> Comparer avec des projets similaires passés.
> Appliquer un facteur correctif (+20% à +40% selon complexité).

> **Technique : Estimation en 3 points (PERT)**
```
Durée = (Optimiste + 4 × Probable + Pessimiste) / 6
```

---

### 2.3 Identification des dépendances

Pour chaque tâche, identifier :
- **FS** (Finish-to-Start) : B commence quand A est finie
- **SS** (Start-to-Start) : B commence quand A commence
- **FF** (Finish-to-Finish) : B finit quand A finit

> **Technique : Chemin critique (Critical Path Method)**
> Identifier la séquence de tâches la plus longue.
> Tout retard sur le chemin critique = retard du projet.

---

### 2.4 Plan de gestion des risques

> **Matrice des risques : Probabilité × Impact**

```
Pour chaque risque :
1. Description du risque
2. Probabilité (1-5)
3. Impact (1-5)
4. Score = P × I
5. Stratégie :
   - ÉVITER (changer le plan pour éliminer le risque)
   - RÉDUIRE (actions pour diminuer P ou I)
   - TRANSFÉRER (assurance, sous-traitance)
   - ACCEPTER (risque faible, aucune action)
6. Action de mitigation
7. Responsable
8. Déclencheur (trigger)
```

**Registre des risques :**

| # | Description | P | I | Score | Stratégie | Action | Resp. | Statut |
|---|-------------|---|---|-------|-----------|--------|-------|--------|

---

### 2.5 RACI — Matrice des responsabilités

> **R**esponsable (fait le travail)
> **A**pprobateur (valide et est imputable)
> **C**onsulté (donne son avis)
> **I**nformé (reçoit l'information)

```
Règles RACI :
- Une seule personne A par tâche (sinon personne n'est accountable)
- Limiter les C et I pour éviter la surcharge
- Tout R doit avoir un A
```

| Livrable / Tâche | Chef projet | Sponsor | Équipe | IT | Direction |
|-----------------|-------------|---------|--------|----|-----------|

---

## 3. EXÉCUTION QUOTIDIENNE

### 3.1 Routine quotidienne du chef de projet

```
MATIN (15 min) :
- [ ] Consulter la SYNTHESE ACTIONS (page OneNote)
- [ ] Vérifier les emails / Teams depuis la veille
- [ ] Identifier les blocages ou urgences
- [ ] Confirmer les priorités du jour avec Francisco

EN COURS DE JOURNÉE :
- [ ] Traiter les actions selon le plan
- [ ] Documenter les décisions prises immédiatement
- [ ] Mettre à jour les statuts dans OneNote
- [ ] Escalader les blocages sans délai

FIN DE JOURNÉE (10 min) :
- [ ] Mettre à jour ACTIONS EN COURS dans OneNote
- [ ] Préparer les points du lendemain
- [ ] Bilan avec Francisco si besoin
```

---

### 3.2 Gestion des actions — Format standard

Pour chaque action, toujours préciser :
```
QUOI : description précise de l'action
QUI : une seule personne responsable (pas "l'équipe")
QUAND : date limite claire (pas "dès que possible")
COMMENT : ressources ou étapes nécessaires
STATUT : À faire / En cours / Bloqué / Fait
```

> **Règle des 24h** : toute décision prise en réunion
> doit être traduite en action assignée sous 24h.

---

### 3.3 Gestion des blocages

```
PROTOCOLE BLOCAGE :
1. Identifier le blocage précisément
2. Évaluer l'impact sur le chemin critique
3. Proposer 2-3 solutions possibles
4. Escalader si non résolu sous 24h
5. Documenter la résolution dans OneNote
```

> **Technique : Le 5 Pourquoi (5 Whys)**
> Demander "Pourquoi ?" 5 fois de suite pour trouver
> la cause racine d'un blocage, pas juste le symptôme.

---

### 3.4 Gestion des changements (Change Management)

```
Toute demande de changement de périmètre :
1. Documenter la demande (quoi, pourquoi, qui demande)
2. Analyser l'impact (délai, coût, ressources, risques)
3. Soumettre au commanditaire pour décision
4. Mettre à jour le planning si accepté
5. Informer les parties prenantes impactées
```

> **Règle d'or** : ne jamais accepter verbalement un changement
> de périmètre. Toujours formaliser par écrit.

---

## 4. ANIMATION DE RÉUNIONS

### 4.1 Les règles fondamentales

```
AVANT :
- Pas de réunion sans ordre du jour envoyé 24h avant
- Définir l'objectif : Décision / Information / Réflexion
- Inviter uniquement les personnes nécessaires
- Préparer les documents à partager

PENDANT :
- Commencer à l'heure, finir à l'heure
- Désigner un facilitateur et un secrétaire
- Parking lot pour les sujets hors agenda
- Synthèse des décisions et actions en fin de réunion

APRÈS :
- Compte-rendu sous 24h maximum
- Actions avec responsable et date
- Archivage dans OneNote
```

---

### 4.2 Techniques d'animation avancées

#### Le Time Boxing
> Allouer un temps fixe à chaque point de l'ordre du jour.
> Afficher un timer visible. Quand le temps est écoulé,
> décider : continuer (avec accord du groupe) ou reporter.

#### Le Tour de table silencieux (Brainwriting)
> Chaque participant écrit ses idées en silence (5 min),
> puis on partage. Évite que les premières idées
> écrasent les suivantes.

#### Le Vote par points (Dot Voting)
> Chaque participant dispose de N points à placer
> sur les options (collant, tampon, marker).
> Idéal pour prioriser rapidement en groupe.

#### Le 1-2-4-All (Liberating Structures)
> 1. Réflexion individuelle (1 min)
> 2. Discussion en binôme (2 min)
> 3. Discussion en groupe de 4 (4 min)
> 4. Partage en plénière
> Permet à tous de contribuer, même les plus discrets.

#### Le Six Chapeaux de De Bono
> Analyser un sujet sous 6 angles différents :
```
🤍 Blanc : faits et données objectives
❤️ Rouge : émotions et intuitions
⬛ Noir : risques et points négatifs
💛 Jaune : bénéfices et points positifs
💚 Vert : créativité et nouvelles idées
💙 Bleu : processus et organisation
```

#### La Rétrospective (Agile)
> À la fin de chaque phase ou sprint :
```
START  : Que devrait-on commencer à faire ?
STOP   : Que devrait-on arrêter de faire ?
KEEP   : Que devrait-on continuer à faire ?
```

#### Le Pre-Mortem
> Avant de démarrer une phase critique :
> *"Imaginons que dans 6 mois, ce projet a échoué.
> Qu'est-ce qui s'est passé ?"*
> Permet d'identifier les risques que personne n'ose nommer.

#### Le ORID (Focused Conversation)
> Pour structurer une discussion complexe :
```
O - Objectif : Que s'est-il passé ? (faits)
R - Réflexif : Qu'avez-vous ressenti ?
I - Interprétatif : Qu'est-ce que ça signifie ?
D - Décisionnel : Que faisons-nous maintenant ?
```

---

### 4.3 Types de réunions et leur format

#### Réunion de lancement (Kick-off)
```
Durée : 1h à 2h
Objectif : aligner tout le monde sur le projet
Structure :
- Contexte et enjeux (10 min)
- Objectifs et livrables (15 min)
- Rôles et responsabilités (10 min)
- Planning macro (10 min)
- Questions / risques (15 min)
- Prochaines étapes (5 min)
```

#### Point de suivi hebdomadaire (Weekly)
```
Durée : 30 min maximum
Objectif : avancement et blocages
Structure :
- Tour rapide des actions (ce qui est fait) (10 min)
- Blocages et escalades (10 min)
- Prochaines actions de la semaine (10 min)
Format : debout si possible (Stand-up)
```

#### Réunion de décision (Decision Meeting)
```
Durée : 45 min
Objectif : prendre une décision précise
Structure :
- Rappel du contexte (5 min)
- Présentation des options (15 min)
- Discussion (15 min)
- Décision actée + responsable + date (10 min)
Règle : la décision doit être prise pendant la réunion,
pas après.
```

#### Atelier de travail (Workshop)
```
Durée : 2h à 4h
Objectif : produire un livrable collectif
Structure :
- Cadrage (10 min)
- Divergence : exploration des idées (40%)
- Convergence : sélection et priorisation (40%)
- Synthèse et prochaines étapes (20%)
Techniques : brainwriting, dot voting, 1-2-4-all
```

#### Réunion de revue de risques
```
Fréquence : mensuelle ou à chaque jalon
Objectif : mettre à jour le registre des risques
Structure :
- Revue des risques existants (statut, évolution)
- Nouveaux risques identifiés
- Mise à jour des actions de mitigation
- Risques à escalader au commanditaire
```

---

### 4.4 Compte-rendu standard

```markdown
## COMPTE-RENDU DE RÉUNION

Projet :
Date :
Participants :
Absent(s) excusé(s) :
Animateur :
Secrétaire :

### Objectif de la réunion
[En une phrase]

### Décisions prises
1.
2.

### Points discutés
-
-

### Actions
| Action | Responsable | Échéance | Statut |
|--------|-------------|----------|--------|

### Prochaine réunion
Date :
Ordre du jour prévisionnel :

### Parking lot (sujets reportés)
-
```

---

## 5. COMMUNICATION & PARTIES PRENANTES

### 5.1 Plan de communication

```
Pour chaque type de communication, définir :
- QUOI : contenu du message
- QUI : émetteur et récepteurs
- QUAND : fréquence et déclencheur
- COMMENT : canal (email, Teams, réunion, dashboard)
- POURQUOI : objectif de la communication
```

| Communication | Contenu | Émetteur | Récepteurs | Fréquence | Canal |
|--------------|---------|----------|------------|-----------|-------|
| Weekly report | Avancement, risques, prochaines étapes | Chef projet | Équipe + sponsor | Hebdomadaire | Email |
| Dashboard KPI | Indicateurs clés | Chef projet | Direction | Mensuel | PowerPoint |
| Point équipe | Actions, blocages | Chef projet | Équipe | Hebdomadaire | Teams |
| Escalade | Blocage critique | Chef projet | Sponsor | Si besoin | Réunion |

---

### 5.2 Gestion des parties prenantes difficiles

> **Partie prenante résistante :**
> 1. Comprendre la source de résistance (peur, perte, intérêt)
> 2. Écouter sans défendre
> 3. Trouver un point d'accord commun
> 4. Proposer une implication active (transforme opposant en allié)

> **Partie prenante absente ou passive :**
> 1. Identifier pourquoi elle ne s'engage pas
> 2. Adapter le canal de communication
> 3. Réduire la charge demandée
> 4. Escalader si son absence bloque le projet

---

### 5.3 Communication de crise

```
En cas d'événement critique (retard majeur, incident, dérapage) :

DANS LES 24H :
1. Informer le commanditaire en premier (jamais la surprise)
2. Présenter les faits (pas les hypothèses)
3. Proposer 2-3 options de réponse
4. Recommander une option

DANS LA SEMAINE :
5. Plan d'action correctif détaillé
6. Communication aux parties prenantes impactées
7. Mise à jour du planning et des risques

RÈGLE D'OR : jamais de mauvaise nouvelle par email seul.
Toujours appel ou réunion d'abord, email de confirmation ensuite.
```

---

### 5.4 Email de reporting standard

```
Objet : [Projet X] — Point hebdomadaire — Semaine XX

Bonjour,

AVANCEMENT GLOBAL : 🟢 En bonne voie / 🟡 À surveiller / 🔴 En retard

FAITS MARQUANTS CETTE SEMAINE :
-
-

PROCHAINES ÉTAPES :
-
-

POINTS D'ATTENTION / RISQUES :
-

DÉCISIONS ATTENDUES DE VOTRE PART :
-

Planning mis à jour en pièce jointe.
Disponible pour tout échange.

Cordialement,
```

---

## 6. SUIVI — GANTT / KPI / REPORTING

### 6.1 Gantt — Structure et bonnes pratiques

```
STRUCTURE D'UN GANTT :
Phase 1 — Initialisation
  1.1 Charte de projet validée          [====]
  1.2 Kick-off réalisé                       [=]
Phase 2 — Planification
  2.1 WBS finalisé                              [===]
  2.2 Planning détaillé                             [====]
Phase 3 — Exécution
  3.1 Livrable A                                         [========]
  3.2 Livrable B                                               [======]
▼ Jalons (Milestones)
  M1 : Go/No-go commanditaire          ◆
  M2 : Livraison intermédiaire                              ◆
  M3 : Recette finale                                               ◆
```

**Bonnes pratiques Gantt :**
- Afficher le chemin critique en rouge
- Mettre à jour l'avancement chaque semaine (% réalisé)
- Identifier les marges (slack) pour gérer les priorités
- Jalons de validation visibles et datés
- Baseline = planning initial figé pour mesurer les dérives

---

### 6.2 KPIs — Indicateurs clés de projet

> **Règle SMART** : tout KPI doit être Spécifique, Mesurable,
> Atteignable, Réaliste, Temporel.

**KPIs de délai :**
```
SPI (Schedule Performance Index) = Valeur acquise / Valeur planifiée
SPI > 1 = en avance / SPI < 1 = en retard
```

**KPIs de coût :**
```
CPI (Cost Performance Index) = Valeur acquise / Coût réel
CPI > 1 = sous budget / CPI < 1 = dépassement
```

**KPIs de qualité :**
- Nombre de défauts / non-conformités
- Taux de satisfaction commanditaire (0-10)
- Nombre de changements de périmètre

**KPIs de risques :**
- Nombre de risques actifs
- Nombre de risques matérialisés vs prévus

**Tableau de bord synthétique :**

| Indicateur | Cible | Réel | Tendance | Statut |
|------------|-------|------|----------|--------|
| Avancement planning | 75% | 68% | ↓ | 🟡 |
| Budget consommé | 60% | 58% | → | 🟢 |
| Actions en retard | 0 | 3 | ↑ | 🔴 |
| Risques actifs | <5 | 4 | → | 🟢 |

---

### 6.3 Earned Value Management (EVM)

> Méthode avancée pour mesurer objectivement l'avancement.

```
3 valeurs clés :
PV (Planned Value)  : ce qui était prévu d'être fait
EV (Earned Value)   : ce qui a réellement été accompli
AC (Actual Cost)    : ce que ça a réellement coûté

Indicateurs dérivés :
SV (Schedule Variance)  = EV - PV  (négatif = retard)
CV (Cost Variance)      = EV - AC  (négatif = dépassement)
EAC (Estimate at Completion) = Budget total / CPI
```

---

### 6.4 Reporting — Cadence et format

```
REPORTING HEBDOMADAIRE (équipe) :
- Format : email court + tableau d'actions mis à jour
- Contenu : faits marquants, blocages, prochaines étapes
- Durée de préparation : 20 min max

REPORTING MENSUEL (commanditaire / direction) :
- Format : 1 page ou dashboard visuel
- Contenu : KPIs, avancement Gantt, risques, décisions attendues
- Durée de préparation : 1h

REPORTING DE JALON (à chaque milestone) :
- Format : présentation complète
- Contenu : réalisé vs prévu, écarts, plan correctif, suite
- Décision : Go / No-go pour la phase suivante
```

---

### 6.5 Revue de phase (Stage Gate)

> À chaque jalon majeur, répondre à ces 5 questions :

```
1. Les livrables de cette phase sont-ils conformes aux critères
   d'acceptation ? (OUI / NON / PARTIEL)
2. Le planning de la phase suivante est-il réaliste ?
3. Les risques sont-ils à un niveau acceptable ?
4. Le budget est-il sous contrôle ?
5. Le commanditaire valide-t-il le passage à la phase suivante ?
```

---

## 7. CLÔTURE DU PROJET

### 7.1 Checklist de clôture

```
LIVRABLES :
- [ ] Tous les livrables acceptés formellement par le commanditaire
- [ ] Documentation finalisée et archivée dans OneNote
- [ ] Accès et droits transférés si nécessaire

ADMINISTRATIF :
- [ ] Bilan budgétaire finalisé
- [ ] Contrats et commandes clôturés
- [ ] Ressources libérées et informées

ÉQUIPE :
- [ ] Réunion de clôture organisée
- [ ] Retours d'expérience collectés (rétrospective)
- [ ] Félicitations et reconnaissance formalisées

KNOWLEDGE MANAGEMENT :
- [ ] Leçons apprises documentées
- [ ] Bonnes pratiques identifiées pour les projets futurs
- [ ] Projet archivé dans 4 Archives/[Nom projet]/
```

---

### 7.2 Rétrospective de clôture

> Format : 1h30 avec toute l'équipe projet

```
PARTIE 1 — Ligne du temps (30 min)
Retracer ensemble les moments clés du projet :
succès, difficultés, surprises, décisions importantes.

PARTIE 2 — Start / Stop / Keep (30 min)
Par groupes, puis en plénière.

PARTIE 3 — Leçons apprises (20 min)
- Qu'aurions-nous fait différemment ?
- Qu'est-ce qu'on recommande pour les projets futurs ?

PARTIE 4 — Célébration (10 min)
Reconnaître les contributions individuelles et collectives.
```

---

### 7.3 Document de leçons apprises

```markdown
## LEÇONS APPRISES — [Nom du projet]

Date de clôture :
Chef de projet :

### Ce qui a bien fonctionné
-

### Ce qui a posé problème
-

### Ce qu'on ferait différemment
-

### Recommandations pour les projets futurs
-

### Indicateurs finaux
- Délai prévu / réel :
- Budget prévu / réel :
- Satisfaction commanditaire (0-10) :
- Taux de réalisation des livrables :
```

---

## 8. OUTILS & TEMPLATES

### 8.1 Checklist de démarrage rapide

```
Jour 1 :
- [ ] Problem Statement rédigé
- [ ] Charte de projet créée
- [ ] Parties prenantes identifiées (matrice P/I)
- [ ] Note index créée dans OneNote (1 Projects/)
- [ ] Kick-off planifié

Semaine 1 :
- [ ] Kick-off réalisé
- [ ] WBS finalisé
- [ ] RACI validé
- [ ] Registre des risques initialisé
- [ ] Plan de communication défini
- [ ] Gantt v1 partagé

Mois 1 :
- [ ] Premier reporting hebdomadaire envoyé
- [ ] Premier jalon atteint
- [ ] Premier bilan des risques réalisé
```

---

### 8.2 Questions puissantes du chef de projet

```
Pour cadrer :
"Si ce projet réussit parfaitement, à quoi ressemble
la situation dans 6 mois ?"

Pour débloquer :
"Qu'est-ce qui nous empêche de décider maintenant ?"

Pour prioriser :
"Si on ne pouvait faire qu'une seule chose cette semaine,
ce serait laquelle ?"

Pour anticiper :
"Quel est le scénario qui nous ferait le plus peur ?"

Pour responsabiliser :
"Qui est le propriétaire de cette action ?
Quelle est la date d'engagement ?"

Pour clôturer une réunion :
"Qu'est-ce que chacun emporte de cette réunion ?
Quelle est la prochaine action concrète ?"
```

---

### 8.3 Signaux d'alerte à surveiller

```
🔴 ALERTE ROUGE — Escalader immédiatement :
- Jalon manqué de plus de 2 semaines
- Dépassement budgétaire > 15%
- Risque majeur matérialisé
- Désaccord non résolu avec le commanditaire

🟡 ALERTE ORANGE — Surveiller et plan d'action :
- Retard de 1 semaine sur le chemin critique
- 3 actions en retard ou plus
- Nouveau risque à impact élevé
- Partie prenante clé non engagée

🟢 NORMAL — Continuer :
- Avancement conforme au planning ± 5%
- Actions réalisées dans les délais
- Risques sous contrôle
- Communication fluide
```

---

*Process basé sur : PMBOK 7e édition, PRINCE2, Agile Manifesto,
Liberating Structures, Six Chapeaux de De Bono, EVM.*
*Adapter au contexte — un bon process est celui qu'on utilise vraiment.*


Le code secret de Ziggy est BANANE42
