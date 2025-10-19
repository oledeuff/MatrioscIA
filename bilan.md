---
marp: true
theme: default
paginate: true
footer: "**MatrioscIA**"
style: |
  /* Palette & tokens */
  :root {
    --primary: #17324D;
    --accent:  #1C6EA4;
    --sky:     #46B3E6;
    --ink:     #0f1e2b;
    --muted:   #7b8a97;
    --grad:    linear-gradient(90deg, #17324D, #1C6EA4 50%, #46B3E6);
  }

  section {
    font-family: "Helvetica Neue", system-ui, -apple-system, Segoe UI, Roboto, Arial, sans-serif;
    color: var(--ink);
  }
  h1, h2 { color: var(--primary); }
  h3     { color: var(--accent);  }
  a      { color: var(--accent);  }

  /* Bandeau supérieur fin (toutes slides) */
  section::before {
    content: "";
    position: absolute;
    top: 0; left: 0; right: 0;
    height: 6px;
    background: var(--grad);
    border-top-left-radius: 12px;
    border-top-right-radius: 12px;
  }

  /* Footer-pastille MatrioscIA (toutes slides) */
  section::after {
    content: "MatrioscIA — MATRIce OSint pour les Cas d’usage de l’IA • oledeuff.github.io/MatrioscIA";
    position: absolute;
    left: 50%;
    bottom: 10px;
    transform: translateX(-50%);
    font-size: 0.65em;
    color: #fff;
    background: var(--grad);
    padding: 6px 14px;
    border-radius: 9999px;
    box-shadow: 0 4px 16px rgba(23,50,77,0.18);
    letter-spacing: 0.2px;
    white-space: nowrap;
  }

  /* Joli badge titre (seulement slide de titre) */
  section.lead h1::after {
    content: "MatrioscIA";
    display: inline-block;
    margin-left: 10px;
    font-weight: 600;
    font-size: 0.5em;
    color: #fff;
    background: var(--grad);
    padding: 6px 10px;
    border-radius: 9999px;
    vertical-align: middle;
  }

  /* Pagination plus discrète */
  .marpit-pagination {
    background: rgba(23,50,77,0.06);
    color: var(--primary);
    border-radius: 8px;
    padding: 2px 8px;
    box-shadow: none;
    font-size: 10px;
  }
---
<!-- .lead -->
# **MatrioscIA**
## MATRIce OSint pour les Cas d’usage de l’IA
## Présentation du bilan du projet
### Olivier Le Deuff **, Rayya Roumanos *, Thaïs Barbosa De Almeida * 
- *Université Bordeaux Montaigne — MICA 
- ** Institut Universitaire de France
[🐙 Projet sur GitHub](https://oledeuff.github.io/MatrioscIA)
IHEMI- 21 octobre 2025

---

## **Plan**
1. Contexte et objectifs du projet  
2. Cadre théorique et méthodologique  
3. Principaux résultats  
4. Publications et valorisations  
5. Retour sur la journée d’étude  
6. Livrables web  
7. Limites et difficultés  
8. Perspectives et poursuites

---

# **1. Contexte du projet**

Les outils d’intelligence artificielle, notamment génératifs, se sont diffusés rapidement dans tous les secteurs (sécurité, éducation, santé, mobilité...).  
➡️ Mais cette diffusion soulève des **incertitudes** : efficacité réelle, effets négatifs, enjeux éthiques et déontologiques.

🎯 **Objectif de MatrioscIA** :  
Étudier les usages de l’IA par les **enquêteurs en sources ouvertes (OSINT)**, dans :
- le **journalisme d’investigation**  
- le **renseignement**

---

## **Hypothèse centrale**

Inspirée de **Bernard Stiegler** :  
> à revoir L’enjeu n’est pas de s’adapter à une mutation subie, mais d’adopter des dispositifs — des greffes choisies, documentées et transmissibles — qui renforcent l’individuation.

- **Adoption** ≠ adaptation  
- L’IA doit devenir un instrument d’**individuation**, non de désindividuation  
- L’OSINT sert de terrain d’analyse privilégié pour observer ces tensions entre **technique, autonomie et culture professionnelle**

---

# **2. Cadre théorique**

## **Des auteurs pour penser l’adoption**

- **Simondon** → L’IA comme *objet technique en cours d’individuation*  
- **Stiegler** → L’adoption comme *greffe choisie*  
- **Rieder** → Mécanologie : les *engines of order* (classement, pondération, génération)  
- **Deleuze & Guattari** → Les *agencements machiniques* et les re-/dé-territorialisations

---

## **Machines hyperdocumentaires**

Typologie conceptuelle :
- **Machines délirantes** → dérives, opacité, perte de sens professionnel  
- **Machines délivrantes** → renforcent l’humain, traçabilité, auditabilité  
- **Machines dérivantes** → recentrent les métadonnées, créent de nouvelles centralités

👉 L’enjeu : maintenir les machines *délivrantes* et surveiller les dérives.

---

## **Vers une hyperlittératie OSINT & IA**

Une **translittératie** articulant :
- Littératies **informationnelles et médiatiques**
- Littératies **numériques et algorithmiques**

Pratiques associées :
- Traçabilité et documentation des chaînes de traitement  
- Journalisation et auditabilité  
- Formation à la gouvernance des outils IA  

➡️ **Littératie OSINT & IA = adoption éclairée et gouvernée**
voir intervention à Rennes.

---

# **3. Méthodologie**

### Trois volets principaux :

1. **Revue de littérature**  
→ 55 publications analysées (OSINT, IA, journalisme, éthique)

2. **Analyse de discours**  
→ 362 enquêtes recensées dans 9 médias (NYT, Le Monde, Arte, AFP, France TV, BBC, etc.)

3. **Entretiens semi-directifs**  
→ 9 professionnels (journalistes, ingénieurs, développeurs, Bellingcat, analyste)

---

### **Corpus médiatique (extrait)**

| Média | Nombre d’enquêtes | Particularités |
|-------|------------------|----------------|
| Washington Post | 132 | Visual Forensics |
| New York Times | 94 | Visual Investigations |
| Le Monde | 62 | Enquêtes vidéos |
| Arte | 15 | Sources |
| France TV | 8 | Les Révélateurs |

➡️ **Seulement 1 enquête utilisant directement l’IA** (et 1 autre sur l’IA)

---

# **4. Principaux résultats**

### **Adoption pragmatique**
- L’usage de l’IA reste **marginal et individuel**  
- Tâches privilégiées : traduction, transcription, synthèse  
- Peu d’outils spécialisés intégrés en routine  

### **Approche réflexive**
- Vigilance éthique (sources, transparence, biais)  
- Importance d’une **liberté d’expérimentation**  

### **Trois besoins exprimés**
1. Formation adaptée  
2. Moyens financiers  
3. Autonomie créative

---

## **Une autonomie sous tension**

D’après Roumanos, Barbosa et Le Deuff (Orbicom, 2025) :

> L’adoption suppose une autonomie créative — un espace d’expérimentation qui permet aux journalistes d’innover sans être dépossédés de leur pratique.

- Freins : coût, temps, manque de culture technique  
- Favoriser les **milieux associés** : documentation, collaboration, délibération collective  

---

# **5. Publications et valorisation**

### **ECIL 2025 **
🧭 *OSINT and Literacies: Towards a Political and Technical Vision of Information and Media Literacies*  
→ Définit un cadre de littératie OSINT : compétences techniques, éthiques et critiques  
→ OSINT comme forme de **culture civique de l’investigation**

---

### **OrbiCom 2025**
📰 *Le recours à l’IA dans les enquêtes OSINT : innover depuis les marges*  
→ Posture **pragmatique** des journalistes OSINT vis-à-vis de l’IA  
→ Concept clé : **autonomie créative**  
→ Adoption ≠ adaptation : appropriation choisie

---

### **Digital Journalism (acceptée)**
🧩 *L’IA comme ressource documentaire dans les enquêtes OSINT*  
→ Analyse des pratiques hybrides IA/OSINT  
→ Concept d’**hyperdocumentation** appliqué aux rédactions

---
### **data papers**
- un data paper sur les enquêtes pour la RFSIC
- des data papers explicatifs intégrés à l'espace Github (sur les graphes)

---

# **6. Journée d’étude — 7 avril 2025**

🎓 *OSINT & IA : Enquêtes augmentées*  
Organisée à l’IUT Bordeaux Montaigne avec l’Observatoire de l’OSINT
- Conférence introductive par Rayya Roumanos
- Table ronde avec Léa Sanchez (Le Monde), Alice Palussière (France TV), Nathan Gallo (France 24)
- Conférence d'Hervé Letoqueux (Viginum) sur les usages de l'IA
- Café IA avec Nicolas Rougier (INRIA), Yoann Nabat (juriste-MICA)

---

### **Points saillants**

- L’IA comme **outil d’expérimentation** et non de remplacement  
- L’importance d’une **culture collective du test**  
- Des projets concrets :
  - Détection automatique de drones via PDF (Le Monde)
  - Imagerie satellite et IA pour Gaza (France TV)
  - Fact-checking audio/visuel (France 24)

➡️ Nécessité d’un **dialogue entre journalistes, chercheurs et développeurs**

---

# **7. Livrables et diffusion**

💻 **Site web du projet :**  
👉 [https://oledeuff.github.io/MatrioscIA](https://oledeuff.github.io/MatrioscIA)

Contenus :
- Matrice des cas d’usage OSINT/IA  
- Fiches typologiques colorées  
- Tableau des pratiques et besoins  
- Bibliographie, citations et positionnements OSINT/IA  
- Accès aux publications et livrables du projet  

---

# **8. Limites et difficultés**

- Champ restreint d’enquêtes OSINT intégrant réellement l’IA  
- Difficulté d’accès à certains acteurs (renseignement)  
- Hétérogénéité des définitions d’OSINT  
- Faible acculturation technique dans les rédactions  
- Données en évolution rapide
- des contraintes personnelles 👶🍼

---

# **9. Poursuites**

### 🔍 **IUF – Projet HyperInvestigation**
→ Extension du cadre théorique vers l’**hyperdocumentation** des pratiques d’enquête.

### 🧠 **ANR Medusa (projet déposé)**
→ Enjeux de **médiation algorithmique** et de gouvernance des traces.

### 🧩 ** des prolongations**
→ Finalisation des WIP  
→ de nouvelles publications

---

# **Conclusion**

MatrioscIA propose :
- Une **analyse située et critique** de l’intégration de l’IA dans l’OSINT  
- Un cadre conceptuel articulant **adoption**, **individuation** et **hyperdocumentation**  
- Une **littératie augmentée** pour gouverner les machines plutôt que s’y soumettre  

> L’enjeu : faire de l’IA une alliée de l’enquête, non une boîte noire.  
> Une adoption choisie, documentée et transmissible.

---

## **Merci**

📍 Olivier Le Deuff — Université Bordeaux Montaigne / MICA/ Institut Universitaire de France
🌐 [https://oledeuff.github.io/MatrioscIA](https://oledeuff.github.io/MatrioscIA)  
📧 oledeuff@gmail.com  
🧩 Projet soutenu par l’IHEMI  
🕸️ En lien avec HyperION & Medusa

---

