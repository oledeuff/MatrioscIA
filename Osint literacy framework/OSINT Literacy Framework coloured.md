# OSINT Literacy Framework — Themed Tree (Flowchart, Colored)

This diagram presents the six core areas of the OSINT Literacy Framework,  
with specific skills, descriptions, examples, and proficiency levels.  
Colors distinguish each thematic entry.

```mermaid
flowchart TB
  R([OSINT Literacy Framework]):::root

  R --> IG[📥 Information Gathering]:::gather
  R --> SE[🕵️ Source Evaluation & Verification]:::verify
  R --> AS[📊 Analysis & Synthesis]:::analyze
  R --> TP[⚙️ Tools & Techniques Proficiency]:::tools
  R --> ES[🔐 Ethics • Legality • Security (OPSEC)]:::ethics
  R --> CT[🧠 Critical Thinking & Reflexivity]:::critical

  %% IG
  IG --> IGs[Specific skills:\n• Targeted queries (Google, Bing, dorks)\n• Social platforms & open/public databases\n• Archives, scraping & automation\n• Data archiving]:::gather
  IG --> IGd[Description:\nEfficiently collect relevant open data]:::gather
  IG --> IGe[Examples:\n• Google Advanced → hidden PDFs\n• Query social media with keywords]:::gather
  IG --> IGl[Level:\nLevel 2 — Good proficiency]:::gather

  %% SE
  SE --> SEs[Specific skills:\n• Authenticity checks (images, videos, docs)\n• Credibility assessment\n• Cross-checking across sources]:::verify
  SE --> SEd[Description:\nValidate sources & information]:::verify
  SE --> SEe[Examples:\n• Reverse image search\n• Cross-check datasets]:::verify
  SE --> SEl[Level:\nLevel 2 — Good proficiency]:::verify

  %% AS
  AS --> ASs[Specific skills:\n• Graphs • maps • timelines\n• Detect links • trends • anomalies\n• Visualization for patterns]:::analyze
  AS --> ASd[Description:\nTurn raw info into intelligence]:::analyze
  AS --> ASe[Examples:\n• Map entities & connections\n• Cross-ref geo & socio-economic data]:::analyze
  AS --> ASl[Level:\nLevel 2 — Good proficiency]:::analyze

  %% TP
  TP --> TPs[Specific skills:\n• Maltego • Shodan • SpiderFoot\n• Specialized platforms • APIs\n• Automation • AI-assisted]:::tools
  TP --> TPd[Description:\nUse tools to optimize processes]:::tools
  TP --> TPe[Examples:\n• Maltego relations graph\n• API-based collection]:::tools
  TP --> TPl[Level:\nLevel 2 — Good proficiency]:::tools

  %% ES
  ES --> ESs[Specific skills:\n• GDPR • copyright • ToS\n• VPN • anonymity • secure browsing]:::ethics
  ES --> ESd[Description:\nEnsure safe, legal, ethical OSINT]:::ethics
  ES --> ESe[Examples:\n• Use a VPN\n• Verify licences before reuse]:::ethics
  ES --> ESl[Level:\nLevel 2 — Good proficiency]:::ethics

  %% CT
  CT --> CTs[Specific skills:\n• Detect biases\n• Review hypotheses\n• Reflective process & clear reporting]:::critical
  CT --> CTd[Description:\nJustify reasoning • show limits • transparency]:::critical
  CT --> CTe[Examples:\n• Publish with verifiable sources & traces]:::critical
  CT --> CTl[Level:\nLevel 3 — Critical capability]:::critical

  %% Theme (GitHub-safe)
  classDef root fill:#ffffff,stroke:#444,color:#222,stroke-width:2px;
  classDef gather  fill:#FFF7CC,stroke:#FFCC00,color:#222,stroke-width:2px;
  classDef verify  fill:#FFE6D5,stroke:#FF6F00,color:#222,stroke-width:2px;
  classDef analyze fill:#E8F0FF,stroke:#1A73E8,color:#222,stroke-width:2px;
  classDef tools   fill:#ECE8FF,stroke:#5C3DFF,color:#222,stroke-width:2px;
  classDef ethics  fill:#EAF7EF,stroke:#2E9E44,color:#222,stroke-width:2px;
  classDef critical fill:#FDE7EF,stroke:#D6336C,color:#222,stroke-width:2px;
