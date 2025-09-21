# 🧩 OSINT Literacy Framework — Mermaid Mindmap

This mindmap summarizes the six core skill areas of the OSINT Literacy Framework,  
including specific skills, descriptions, examples, and proficiency levels.

# OSINT Literacy Framework — Themed Mindmap (Colored)

```mermaid
mindmap
  root((OSINT Literacy Framework)):::root

    IG(📥 Information Gathering):::gather
      Specific skills:::gather
        Targeted queries (Google, Bing, dorks):::gather
        Social platforms & open/public databases:::gather
        Archives, scraping & automation:::gather
        Data archiving:::gather
      Description:::gather
        Efficiently collect relevant open data:::gather
      Examples:::gather
        Google Advanced → hidden PDFs:::gather
        Query social media with keywords:::gather
      Level:::gather
        Level 2 — Good proficiency:::gather

    SE(🕵️ Source Evaluation & Verification):::verify
      Specific skills:::verify
        Authenticity checks (images, videos, docs):::verify
        Credibility assessment:::verify
        Cross-checking across sources:::verify
      Description:::verify
        Validate sources & information:::verify
      Examples:::verify
        Reverse image search:::verify
        Cross-check datasets:::verify
      Level:::verify
        Level 2 — Good proficiency:::verify

    AS(📊 Analysis & Synthesis):::analyze
      Specific skills:::analyze
        Graphs • maps • timelines:::analyze
        Detect links • trends • anomalies:::analyze
        Visualization for patterns:::analyze
      Description:::analyze
        Turn raw info into intelligence:::analyze
      Examples:::analyze
        Map entities & connections:::analyze
        Cross-ref geo & socio-economic data:::analyze
      Level:::analyze
        Level 2 — Good proficiency:::analyze

    TP(⚙️ Tools & Techniques):::tools
      Specific skills:::tools
        Maltego • Shodan • SpiderFoot:::tools
        Specialized platforms • APIs:::tools
        Automation • AI-assisted processing:::tools
      Description:::tools
        Use tools to optimize processes:::tools
      Examples:::tools
        Maltego for relations graph:::tools
        API-based collection:::tools
      Level:::tools
        Level 2 — Good proficiency:::tools

    ES(🔐 Ethics • Legality • Security):::ethics
      Specific skills:::ethics
        GDPR • copyright • ToS:::ethics
        VPN • anonymity • secure browsing:::ethics
      Description:::ethics
        Ensure safe, legal, ethical OSINT:::ethics
      Examples:::ethics
        Use a VPN:::ethics
        Verify licences before reuse:::ethics
      Level:::ethics
        Level 2 — Good proficiency:::ethics

    CT(🧠 Critical Thinking & Reflexivity):::critical
      Specific skills:::critical
        Detect biases:::critical
        Review hypotheses:::critical
        Reflective process & clear reporting:::critical
      Description:::critical
        Justify reasoning • show limits • transparency:::critical
      Examples:::critical
        Publish with verifiable sources & traces:::critical
      Level:::critical
        Level 3 — Critical capability:::critical

%% === Theming (colors & contrast) ===
classDef root fill:#ffffff,stroke:#444,color:#222,stroke-width:2px;

classDef gather  fill:#FFF7CC,stroke:#FFCC00,color:#222,stroke-width:2px;
classDef verify  fill:#FFE6D5,stroke:#FF6F00,color:#222,stroke-width:2px;
classDef analyze fill:#E8F0FF,stroke:#1A73E8,color:#222,stroke-width:2px;
classDef tools   fill:#ECE8FF,stroke:#5C3DFF,color:#222,stroke-width:2px;
classDef ethics  fill:#EAF7EF,stroke:#2E9E44,color:#222,stroke-width:2px;
classDef critical fill:#FDE7EF,stroke:#D6336C,color:#222,stroke-width:2px;
