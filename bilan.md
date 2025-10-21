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
Mais cette diffusion soulève des incertitudes : efficacité réelle, effets négatifs, enjeux éthiques et déontologiques.

**Objectif de MatrioscIA** :  
Étudier les usages de l’IA par les **enquêteurs en sources ouvertes (OSINT)**, dans :
- le **journalisme d’investigation**  
- le **renseignement**

---
# **2. Cadre théorique**

## **Des auteurs pour penser l’adoption**

- **Simondon** → L’IA comme *objet technique en cours d’individuation* (+ individuation psychique et collective) 
- **Stiegler** → L’adoption comme *greffe choisie*  
- **Rieder** → Mécanologie à la suite de Simondon : les *engines of order* (classement, pondération, génération) sont des machines de pouvoir  
- **Deleuze & Guattari** → Les *agencements machiniques* précèdent leur concrétisation technique. Les fameuses *machines désirantes*

---
## **Hypothèse centrale** 

Inspirée de **Bernard Stiegler** et **ars industrialis** 
> “Adoption est un terme qui dérive d’« ad-optare » qui signifie opter ou choisir, greffer ou acquérir. Toute individuation humaine est un processus d’adoption, et la santé d’une individuation se mesure à sa possibilité d’adoption – d’un mode de vie, d’une technique, d’une idée, d’un étranger, etc. Le « faire sien » qu’est l’adoption suppose une participation de ce qui adopte à ce qui est adopté. Adapter/adopter. L’adoption est le processus d’une individuation, c’est à dire d’un enrichissement, tandis que l’adaptation est une désindividuation : une restriction des possibilités de l’individu.”

---
## **Adoption** ≠ adaptation  
- examens des rapports à l'IA 
- L’OSINT sert de terrain d’analyse privilégié pour observer ces tensions entre **technique, autonomie et culture professionnelle**
- mesure aussi du degré potentiel d'**institutionnalisation**

---

## **Hyperdocumentation**
 > « L’homme n’aurait plus besoin de documentation s’il était assimilé à un être devenu omniscient, à la manière de Dieu même. À un degré moins ultime serait créée une instrumentation agissant à distance qui combinerait à la fois la radio, les rayons Röntgen, le cinéma et la photographie microscopique. Toutes les choses de l’univers, et toutes celles de l’homme seraient enregistrées à distance à mesure qu’elles se produiraient. Ainsi serait établie l’image mouvante du monde, sa mémoire, son véritable double. Chacun à distance pourrait lire le passage lequel, agrandi et limité au sujet désiré, viendrait se projeter sur l’écran individuel. Ainsi, chacun dans son fauteuil pourrait contempler la création, en son entier ou en certaines de ses parties. P. Otlet. Monde, essai d'universalisme (1935) 

Voir aussi *Traité de documentation* (1934) et Le Deuff, *Hyperdocumentation* (2021)

---

## **Machines hyperdocumentaires**

Typologie conceptuelle :
- **Machines dérivantes** → recentrent les métadonnées, créent de nouvelles centralités
- **Machines délirantes** → dérives, opacité, perte de sens professionnel  
- **Machines délivrantes** → renforcent l’humain, traçabilité, auditabilité  

L’enjeu : adopter les machines *délivrantes* et surveiller les dérives notamment en ce qui concerne les IA.
source : Olivier Le Deuff. *Hyperdocumentation*

---


# **3. Méthodologie**

### Trois volets principaux à la base

1. **Revue de littérature**  
→ 55 publications analysées (OSINT, IA, journalisme, éthique) pour une premier état de l'art.
→ [bibliographie complétée](https://oledeuff.github.io/MatrioscIA/bibliographie)   

2. **Analyse de discours**  
→ 362 enquêtes recensées dans 9 médias (NYT, Le Monde, Arte, AFP, France TV, BBC, etc.)
[site web dédié](https://oledeuff.github.io/MatrioscIA/investigations)
---
# **Méthodologie suite**
3. **Entretiens semi-directifs**  
→ 13 professionnels (journalistes, ingénieurs, développeurs, Bellingcat, analyste)
→ logique immersive (échanges, Festival OSINT, discussions J.E, sollicitations externes, etc.)

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
- Peu d’outils *spécialisés* intégrés en routine  

---

### **Approche réflexive**
- Vigilance éthique (sources, transparence, biais)  
- Importance d’une **liberté d’expérimentation**  
- Dimension critique forte : *pharmacologique* ?

### **Trois besoins exprimés**
1. Formation adaptée  
2. Moyens financiers  
3. Autonomie créative

---

## **Une autonomie sous tension**

Pour les journalistes

> L’adoption suppose une autonomie créative — un espace d’expérimentation qui permet aux journalistes d’innover sans être dépossédés de leur pratique.
Roumanos, Barbosa et Le Deuff (Orbicom, 2025)

- Freins : coût, temps, manque de **culture technique**  
- Favoriser les **milieux associés** (Simondon-Stiegler) : documentation, collaboration, délibération collective  

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
### Pas d'outils miracles mais
- l'IA n'est pas perçue directement comme remède ou poison (le risque du **pharmakon**)
- Mais volonté de gagner du temps et en efficacité
- Envie d'un outil proche de ses besoins personnels:
    - le fantasme de l'outil tout en un prôné et vendu par les développeurs privés
    ... ne se retrouvent pas dans les rédactions ou chez Viginum
    - plutôt un outil qui regroupe des habitudes et des besoins spécifiques selon les profils

---

### Vers une typologie des utilisateurs

| **Profil** | **Description synthétique** |
|:------------|:----------------------------|
| **Médiateurs réflexifs** | Favorisent la réflexion éthique et critique sur les usages de l’IA et des données. |
| **Explorateurs critiques** | Expérimentent les outils d’enquête numérique avec vigilance. Documentent méthodes et biais, transforment la technique en objet d’analyse. |
| **Artisans du récit** | Utilisent l’IA ou l’OSINT au service du récit critique (debunk, expositions, narrations augmentées) sans en faire une fin en soi. |

<!-- _style: |
section {
  font-size: 0.8em;
}
table {
  font-size: 0.85em;
  width: 100%;
}
th {
  background-color: #f3f3f3;
}
--> 
---
| **Profil** | **Description synthétique** |
|:------------|:----------------------------|
|
| **Enquêteurs augmentés** | Exploitent l’IA pour la veille, la traduction ou la rédaction. Visent l’efficacité tout en gardant une supervision humaine. |
| **Gestionnaires techniques** | Assurent l’intégration et la maintenance d’outils IA/OSINT. Veillent à la gouvernance, la sécurité et la standardisation. Approche parfois solutionniste et peu éthique. |
| **Ingénieurs de la preuve** | Développent ou prototypent des outils d’enquête avancés (vision, géoloc, ML). Travaillent dans une logique R&D ouverte et expérimentale. |

<!-- _style: |
section {
  font-size: 0.9em;
}
table {
  font-size: 0.85em;
  width: 100%;
}
th {
  background-color: #f3f3f3;
}
--> 
---
## **Vers une hyperlittératie OSINT & IA**

Une **translittératie** articulant :
- Littératies **informationnelles et médiatiques**
- Littératies **numériques et algorithmiques**
Pratiques associées :
- Traçabilité et documentation des chaînes de traitement  
- auditabilité des systèmes
- Formation à la gouvernance des outils IA (et des données intégrées et produites)

➡️ **Littératie OSINT & IA = adoption éclairée et gouvernée**
voir intervention à Rennes sur les [**hyperlittératies**](https://github.com/oledeuff/Conferences/blob/main/hyperlittératies.pdf)
cadre théorique de base : article sur la littératie algorithmique.

---
# **5. Publications et valorisation**

### **ECIL 2025**
*OSINT and Literacies: Towards a Political and Technical Vision of Information and Media Literacies*  
→ Définit un [référentiel de littératie OSINT](https://oledeuff.github.io/MatrioscIA/framework) : compétences techniques, éthiques et critiques  
→ OSINT comme forme de **culture civique de l’investigation**
→ articulation avec les littératies existantes (notamment IL et ML parmi les anciennes, et les nouvelles Algorithm literacy)

---

### **OrbiCom 2025**
*Le recours à l’IA dans les enquêtes OSINT : innover depuis les marges*  
→ Posture **pragmatique** des journalistes OSINT vis-à-vis de l’IA  
→ Concept clé : **autonomie créative**  
→ Adoption ≠ adaptation : appropriation choisie

---

## **Digital Journalism (proposition acceptée)**
- Processus de **rationalisation** qui précède l'institutionnalisation  
→ Analyse des pratiques hybrides IA/OSINT  
→ Concept d’**hyperdocumentation** appliqué aux rédactions

---
## **Data papers** WIP
- un data paper sur les enquêtes cataloguées pour la RFSIC (en cours de rédaction)
- des data papers explicatifs intégrés à l'espace Github (sur les graphes) (une possible version pour une revue orientée DH)

---

# **6. Journée d’étude — 7 avril 2025**

*OSINT & IA : Enquêtes augmentées*  
Organisée à l’IUT Bordeaux Montaigne avec l’Observatoire de l’OSINT
- Conférence introductive par Rayya Roumanos
- Table ronde avec Léa Sanchez (Le Monde), Alice Palussière (France TV), Nathan Gallo (France 24)
- Conférence d'Hervé Letoqueux (Viginum) sur les usages de l'IA
- Café IA avec Nicolas Rougier (INRIA), Yoann Nabat (juriste-MICA) sur les enjeux politiques, juridiques, éthiques et techniques
    collaborations avec l'**observatoire de la surveillance**.


---

# **7. Livrables et diffusion**

**Site web du projet :**  [https://oledeuff.github.io/MatrioscIA](https://oledeuff.github.io/MatrioscIA)

Contenus :
- Base des enquêtes de type Osint
- catalogue des outils OSINT
- Référentiels OSINT literacy et O& IA literacy
- Graphes de 3 investigations (WIP)
- Matrice des cas d’usage OSINT/IA  
- Citations et positionnements OSINT/IA    
- Bibliographie 


---

# **8. Limites et difficultés**

- Champ restreint d’enquêtes OSINT intégrant réellement l’IA  
- Difficulté d’accès à certains acteurs (renseignement)  
- Hétérogénéité des définitions d’OSINT  
- Faible acculturation technique dans les rédactions  
- Données en évolution rapide
- Des contraintes personnelles 👶🍼

---

# **9. Poursuites**

### **IUF – Projet HyperInvestigation**
→ Extension du cadre théorique vers l’**hyperdocumentation** des pratiques d’enquête.

### **ANR Medusa (projet déposé)** sur Surveillance et journalisme
→ Enjeux de **médiation algorithmique** et de gouvernance des traces.

### **Des prolongations**
→ Finalisation des WIP  
→ des bonus ([personas liés à la matrice](https://oledeuff.github.io/MatrioscIA\personas.html), autoests de positionnement, ludification ?)
→ de nouvelles publications (articles, chapitres, conférences, etc.)
→ des prolongations pédagogiques avec Osint4fun pour l'IUT, et  autres projets avec l'IJBA

---

# **Conclusion**

MatrioscIA propose :
- Une **analyse située et critique** de l’intégration de l’IA dans l’OSINT  
- Un cadre conceptuel articulant **adoption**, **individuation** et **hyperdocumentation**  
- Une **littératie augmentée** pour gouverner les machines plutôt que s’y soumettre  

> L’enjeu : faire de l’IA une alliée de l’enquête, non une boîte noire.  
> Une adoption choisie, documentée et transmissible.
    - au final le travail d'information est fortement lié à sa communication.

Un cadre d'analyse à poursuivre au travers du prisme de l'*hyperinvestigation*

---

## **Merci pour votre attention**

site du projet
🌐 [https://oledeuff.github.io/MatrioscIA](https://oledeuff.github.io/MatrioscIA)  



