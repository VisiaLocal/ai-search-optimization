# AI Search Optimization

## Référentiel 2026 sur la visibilité dans les moteurs de recherche utilisant l'intelligence artificielle

La recherche d'information évolue.

Pendant plusieurs décennies, l'interface dominante de la recherche Web reposait principalement sur une liste de résultats.

Aujourd'hui, plusieurs systèmes peuvent également :

- interpréter une question complexe ;
- lancer plusieurs recherches ;
- récupérer plusieurs documents ;
- extraire des passages ;
- comparer des sources ;
- combiner des informations ;
- générer une réponse ;
- citer ou proposer des sources complémentaires.

Cette évolution ne supprime pas le SEO.

Elle élargit l'environnement dans lequel les informations d'une organisation peuvent être découvertes et utilisées.

Une représentation conceptuelle :

**REAL-WORLD ENTITY**

↓

**FIRST-PARTY DATA**

↓

**BUSINESS KNOWLEDGE**

↓

**CONTENT**

↓

**ENTITIES**

↓

**RELATIONSHIPS**

↓

**STRUCTURED DATA**

↓

**WEB INDEX**

↓

**RETRIEVAL**

↓

**QUERY FAN-OUT**

↓

**RAG / GROUNDING**

↓

**SOURCE SELECTION**

↓

**GENERATED ANSWER**

↓

**CITATIONS / LINKS**

↓

**USER**

↓

**VISIT / CONVERSION**

Ce référentiel propose un cadre permettant de comprendre et d'organiser l'optimisation pour ces nouveaux environnements.

---

# 1. Qu'est-ce que l'AI Search ?

Dans ce référentiel, **AI Search** désigne les expériences de recherche utilisant des modèles d'intelligence artificielle pour aider à comprendre une requête, récupérer de l'information et/ou générer une réponse.

Ces expériences peuvent prendre différentes formes :

- réponse générée ;
- résumé ;
- conversation ;
- comparaison ;
- recommandation ;
- synthèse multi-source ;
- recherche assistée ;
- exploration approfondie.

---

# 2. AI Search ≠ LLM seul

Un modèle de langage et un moteur de recherche utilisant un modèle de langage ne sont pas nécessairement la même chose.

Une expérience AI Search peut combiner :

**MODEL**

+

**SEARCH INDEX**

+

**RETRIEVAL**

+

**EXTERNAL SOURCES**

+

**TOOLS**

+

**RANKING SYSTEMS**

↓

**ANSWER**

Le modèle n'est alors qu'une composante du système.

---

# 3. AI Search ≠ Training Data

Il faut distinguer :

**TRAINING**

et :

**RETRIEVAL**

Un système peut répondre à partir :

- de connaissances apprises pendant l'entraînement ;
- d'informations récupérées au moment de la requête ;
- d'outils ;
- de bases de données ;
- de plusieurs de ces mécanismes.

Publier une page Web ne signifie donc pas automatiquement qu'elle devient immédiatement une connaissance permanente d'un modèle.

---

# 4. Retrieval

Le retrieval consiste à récupérer des ressources pertinentes pour répondre à un besoin informationnel.

Les ressources peuvent inclure :

- pages Web ;
- documents ;
- bases de données ;
- passages ;
- produits ;
- lieux ;
- résultats de recherche.

---

# 5. Retrieval-Augmented Generation

RAG signifie généralement :

**Retrieval-Augmented Generation**

Une architecture simplifiée :

**QUERY**

↓

**RETRIEVAL**

↓

**RELEVANT INFORMATION**

↓

**MODEL CONTEXT**

↓

**GENERATED ANSWER**

L'objectif est notamment de permettre au système de s'appuyer sur des informations externes au modèle.

---

# 6. Grounding

Le grounding consiste à ancrer une réponse dans des informations récupérées ou fournies.

Il peut contribuer à :

- actualité ;
- vérifiabilité ;
- précision ;
- attribution.

Les implémentations diffèrent selon les systèmes.

---

# 7. Query Fan-Out

Une requête complexe peut nécessiter plusieurs recherches.

Exemple :

> Quel hôtel à Aix-en-Provence convient à une famille avec parking, piscine et restaurant ?

Un système peut chercher séparément :

- hôtels Aix-en-Provence ;
- hôtels avec parking ;
- hôtels avec piscine ;
- hôtels familiaux ;
- hôtels avec restaurant.

Puis combiner les résultats.

Ce processus est souvent décrit comme **query fan-out**.

---

# 8. Why Query Fan-Out Matters

Dans une recherche traditionnelle, une page pouvait être principalement optimisée autour d'une requête.

Dans un environnement utilisant plusieurs sous-requêtes, la visibilité peut dépendre d'une couverture informationnelle plus large.

Cela renforce l'intérêt de représenter clairement :

- entités ;
- attributs ;
- relations ;
- services ;
- conditions ;
- preuves.

---

# 9. Complex Queries

Les utilisateurs peuvent formuler des demandes beaucoup plus détaillées.

Exemple :

> Je cherche une agence capable de travailler sur le SEO d'un réseau de commerces, mais aussi sur Google Business Profile, les données structurées et la visibilité dans les moteurs IA.

Cette demande contient plusieurs dimensions.

---

# 10. Query Decomposition

Une demande peut être décomposée en :

**ENTITY TYPE**

agency

**CAPABILITY**

SEO

**BUSINESS MODEL**

multi-location network

**PLATFORM**

Google Business Profile

**TECHNOLOGY**

structured data

**OBJECTIVE**

AI Search visibility

La recherche devient multidimensionnelle.

---

# 11. Keyword Matching vs Information Matching

Une logique Keyword-First cherche principalement :

> La page contient-elle la requête ?

Une logique informationnelle cherche davantage :

> La source contient-elle les informations nécessaires pour répondre ?

Les deux ne sont pas nécessairement opposées.

---

# 12. Information Retrieval

L'Information Retrieval est un domaine historique de l'informatique consacré à la récupération d'informations pertinentes.

AI Search ajoute de nouvelles couches mais ne fait pas disparaître ce problème fondamental.

---

# 13. Documents

Un système peut récupérer un document complet.

Mais il peut également s'intéresser à une partie spécifique de ce document.

---

# 14. Passage Retrieval

Une longue page peut contenir plusieurs passages répondant à différents besoins.

Exemple :

**PAGE**

Semantic SEO

↓

passage 1

definition

↓

passage 2

entities

↓

passage 3

structured data

↓

passage 4

AI Search

La clarté locale des passages devient importante.

---

# 15. Answer Units

Dans le framework VisiaLocal, une **Answer Unit** est une unité de contenu conçue pour répondre clairement à un besoin informationnel identifiable.

Exemple :

### Qu'est-ce que le GEO ?

> Le Generative Engine Optimization regroupe les pratiques visant à améliorer la visibilité et l'utilisation des contenus dans les environnements de recherche générative.

Puis la page peut développer.

---

# 16. Answer Unit ≠ Featured Snippet Hack

Une Answer Unit n'est pas une technique garantissant :

- featured snippet ;
- AI Overview ;
- citation ;
- classement.

Elle constitue avant tout une manière d'organiser l'information.

---

# 17. Answerability

Dans ce framework, **Answerability** désigne la capacité d'une ressource à fournir une réponse suffisamment claire à une question.

Il s'agit d'un concept méthodologique.

Ce n'est pas une métrique officielle d'un moteur.

---

# 18. Search Engine Optimization

SEO signifie :

**Search Engine Optimization**

Le SEO vise notamment à améliorer :

- accessibilité ;
- crawlabilité ;
- indexation ;
- compréhension ;
- pertinence ;
- visibilité.

Ces fondamentaux restent importants dans les environnements AI Search utilisant le Web.

---

# 19. Answer Engine Optimization

AEO signifie généralement :

**Answer Engine Optimization**

Le terme est utilisé pour décrire des pratiques visant à améliorer la capacité d'un contenu à fournir des réponses exploitables dans les moteurs ou interfaces de réponse.

---

# 20. Generative Engine Optimization

GEO signifie :

**Generative Engine Optimization**

Le terme est utilisé pour désigner l'optimisation de contenus et de sources pour les environnements utilisant des réponses génératives.

---

# 21. AI Search Optimization

Dans ce référentiel, **AI Search Optimization** constitue le périmètre le plus large.

Il peut inclure :

**SEO**

+

**AEO**

+

**GEO**

+

**ENTITY OPTIMIZATION**

+

**INFORMATION ARCHITECTURE**

+

**STRUCTURED DATA**

+

**SOURCE STRATEGY**

+

**RETRIEVAL READINESS**

+

**MEASUREMENT**

---

# 22. SEO vs AEO vs GEO vs AI Search Optimization

### SEO

Optimiser la présence dans les moteurs de recherche.

### AEO

Organiser l'information pour faciliter les réponses.

### GEO

Travailler la visibilité dans les environnements génératifs.

### AI Search Optimization

Coordonner l'ensemble des couches pouvant influencer la découverte, la récupération, la compréhension et l'utilisation des informations dans les expériences de recherche utilisant l'IA.

---

# 23. AI Search Is Not One Engine

Il n'existe pas un moteur IA unique.

Les systèmes peuvent différer par :

- index ;
- modèles ;
- fournisseurs de recherche ;
- retrieval ;
- ranking ;
- citations ;
- interface ;
- personnalisation ;
- outils.

Une stratégie ne doit donc pas supposer qu'une technique fonctionne identiquement partout.

---

# 24. Google AI Overviews

Google peut afficher des réponses génératives directement dans Search sous la forme d'AI Overviews.

Ces expériences restent intégrées à l'écosystème Google Search.

---

# 25. Google AI Mode

AI Mode propose une expérience de recherche davantage conversationnelle et générative.

Les mécanismes et fonctionnalités peuvent évoluer.

---

# 26. ChatGPT Search

ChatGPT peut utiliser la recherche Web pour fournir des informations actuelles et proposer des liens vers des sources.

La présence d'une source dans une réponse dépend du contexte de la requête et du système de recherche utilisé.

---

# 27. Gemini

Les expériences Gemini peuvent combiner les capacités des modèles Google avec différents outils et sources selon le produit et le contexte.

Il ne faut pas supposer que toutes les réponses Gemini utilisent exactement le même pipeline.

---

# 28. Perplexity

Perplexity est un exemple d'interface de recherche centrée sur les réponses générées et les sources.

Les mécanismes de sélection peuvent évoluer.

---

# 29. Microsoft Copilot

Microsoft propose également plusieurs expériences utilisant l'IA et la recherche.

Le comportement peut varier selon le produit Copilot concerné.

---

# 30. Search Surface Diversity

Une entreprise peut donc apparaître dans plusieurs environnements :

**TRADITIONAL SEARCH**

↓

**AI OVERVIEW**

↓

**AI MODE**

↓

**CHATGPT SEARCH**

↓

**PERPLEXITY**

↓

**COPILOT**

↓

**OTHER AI SEARCH SYSTEMS**

Une présence universelle ne peut pas être garantie.

---

# 31. Source Selection

Une réponse générative doit parfois sélectionner quelques sources parmi un très grand nombre de documents disponibles.

La question devient alors :

> Pourquoi cette source est-elle suffisamment pertinente pour ce besoin précis ?

Il n'existe pas une réponse universelle.

---

# 32. Relevance

Une source doit contenir des informations pertinentes pour la demande.

La répétition exacte de la requête n'est pas nécessairement le seul moyen d'établir cette pertinence.

---

# 33. Specificity

Une information spécifique peut être plus utile qu'une affirmation générique.

Faible :

> Nous proposons un service rapide.

Plus informatif :

> Les commandes personnalisées validées avant 14 h sont préparées sous 24 heures ouvrées.

La seconde formulation contient davantage d'information exploitable.

---

# 34. Verifiability

Certaines affirmations gagnent à être vérifiables.

Exemple :

> Entreprise certifiée X.

peut être soutenu par :

- organisme certificateur ;
- certificat ;
- registre ;
- source officielle.

---

# 35. Evidence

Une affirmation peut être reliée à :

**CLAIM**

↓

**EVIDENCE**

↓

**SOURCE**

Cette relation est particulièrement importante pour les affirmations fortes.

---

# 36. Source Quality

La qualité d'une source dépend du type d'information recherché.

Pour :

**horaires d'un commerce**

→ source officielle de l'entreprise.

Pour :

**loi**

→ source gouvernementale.

Pour :

**expérience client**

→ avis réels.

Pour :

**recherche scientifique**

→ publication académique.

---

# 37. Primary Sources

Les sources primaires peuvent être particulièrement importantes lorsqu'elles sont disponibles.

Exemples :

- documentation officielle ;
- entreprise concernée ;
- étude originale ;
- registre ;
- données propriétaires.

---

# 38. Secondary Sources

Une source secondaire peut :

- expliquer ;
- contextualiser ;
- comparer ;
- synthétiser.

Elle peut également être très utile.

---

# 39. Independent Sources

Une organisation ne contrôle pas toutes les sources qui parlent d'elle.

Des sources indépendantes peuvent contribuer à confirmer :

- existence ;
- réputation ;
- expertise ;
- événements ;
- partenariats.

---

# 40. Corroboration

Dans ce framework, la corroboration représente la convergence de plusieurs sources compatibles autour d'un même fait.

Exemple :

**OFFICIAL WEBSITE**

↓

Aix-en-Provence

**PROFESSIONAL DIRECTORY**

↓

Aix-en-Provence

**PARTNER PAGE**

↓

Aix-en-Provence

La répétition artificielle n'est pas l'objectif.

---

# 41. Corroboration ≠ Link Building

Une source peut corroborer une information sans nécessairement transmettre un backlink.

La corroboration concerne d'abord la cohérence des informations.

---

# 42. Citation

Dans une réponse générative, une citation peut permettre à l'utilisateur de :

- identifier une source ;
- vérifier l'information ;
- approfondir ;
- visiter le site.

La présentation exacte varie selon les plateformes.

---

# 43. Citation ≠ Ranking

Être cité dans une réponse générative et être classé dans une SERP classique sont deux événements différents.

Ils peuvent néanmoins dépendre de certaines infrastructures communes.

---

# 44. Citation Eligibility

Dans ce framework, **Citation Eligibility** désigne conceptuellement la capacité d'une ressource à constituer une source potentiellement pertinente pour une réponse.

Ce n'est pas une métrique officielle.

---

# 45. Citation Readiness

Une ressource peut améliorer sa Citation Readiness en fournissant :

- informations précises ;
- source identifiable ;
- contexte ;
- date lorsque pertinente ;
- preuves ;
- passages autonomes ;
- cohérence.

Cela ne garantit pas une citation.

---

# 46. Citation Gap

Dans ce framework, un Citation Gap peut exister lorsque :

- l'entreprise possède une information utile ;
- mais aucune ressource publique suffisamment claire ne permet facilement de la sourcer.

---

# 47. Source Gap

Une entreprise peut affirmer quelque chose sans fournir de ressource appropriée pour le vérifier.

Exemple :

> Nous sommes certifiés X.

mais aucune page ni source ne permet de comprendre :

- quelle certification ;
- par qui ;
- quand.

---

# 48. Information Gap

Une information réelle peut exister sans être publiée.

Cette information est alors difficile à récupérer depuis le Web.

---

# 49. Entity Gap

Une entité réelle importante peut être insuffisamment représentée.

Exemple :

une entreprise possède une division spécialisée mais aucune ressource ne permet de comprendre clairement son existence ou sa relation avec l'organisation.

---

# 50. Relationship Gap

Deux entités peuvent être représentées sans que leur relation soit claire.

Exemple :

**Person A**

et

**Company A**

existent en ligne.

Mais aucune source n'indique clairement que Person A est le fondateur de Company A.

---

# 51. Answer Gap

Une question importante peut ne disposer d'aucune réponse claire.

L'information existe peut-être implicitement mais reste difficile à extraire.

---

# 52. Evidence Gap

Une affirmation peut être publiée sans preuve appropriée.

Cela peut réduire sa valeur pour certaines utilisations.

---

# 53. Freshness Gap

Une information peut être exacte historiquement mais obsolète aujourd'hui.

Dans les environnements de recherche actuels, la fraîcheur peut être essentielle selon la requête.

---

# 54. First-Party Data

Une organisation possède des données directement issues de son activité.

Exemples :

- catalogue ;
- services ;
- prix ;
- délais ;
- stock ;
- zones ;
- caractéristiques ;
- statistiques ;
- processus.

---

# 55. First-Party Knowledge

Dans le framework VisiaLocal, **Business First-Party Knowledge** désigne la connaissance factuelle qu'une entreprise possède sur sa propre activité.

Cette connaissance peut constituer une source de contenu original.

---

# 56. Commodity Content

Un contenu générique reproduisant les mêmes informations que des centaines d'autres pages apporte peu de différenciation informationnelle.

---

# 57. Non-Commodity Information

Une entreprise peut posséder des informations que les autres sites ne peuvent pas facilement reproduire :

- données propriétaires ;
- expertise ;
- méthodologie ;
- catalogue ;
- disponibilité ;
- études de cas ;
- résultats ;
- expérience.

Ces informations peuvent augmenter la singularité du corpus.

---

# 58. Information Gain

Une ressource peut apporter un gain informationnel lorsqu'elle fournit quelque chose d'utile qui n'est pas déjà présent partout ailleurs.

---

# 59. Original Information

L'originalité ne signifie pas nécessairement inventer un nouveau concept.

Elle peut provenir de :

- données ;
- observations ;
- expérience ;
- analyse ;
- expertise ;
- documentation.

---

# 60. Entity Modeling

AI Search renforce l'intérêt de représenter clairement :

- qui ;
- quoi ;
- où ;
- comment ;
- avec qui.

Les entités fournissent une structure conceptuelle aux informations.

---

# 61. Organization Entity

Une organisation peut être reliée à :

- site ;
- dirigeants ;
- services ;
- produits ;
- établissements ;
- profils ;
- certifications.

---

# 62. Person Entity

Une personne peut être reliée à :

- organisation ;
- rôle ;
- expertise ;
- publications ;
- projets.

Les relations doivent être réelles.

---

# 63. Service Entity

Un service peut posséder :

- nom ;
- fournisseur ;
- description ;
- zone ;
- audience ;
- conditions ;
- prix.

---

# 64. Product Entity

Un produit peut posséder :

- fabricant ;
- marque ;
- caractéristiques ;
- prix ;
- disponibilité ;
- variantes.

---

# 65. Place Entity

Une entreprise locale peut être reliée à :

- adresse ;
- ville ;
- région ;
- zone de service.

---

# 66. Entity Relationships

Les relations peuvent être plus informatives que les entités isolées.

Exemple :

**ORGANIZATION**

↓

provides

↓

**SERVICE**

↓

availableIn

↓

**PLACE**

---

# 67. Entity Resolution

Un système peut rencontrer plusieurs mentions similaires.

Il doit déterminer si elles correspondent :

- à la même entité ;
- à plusieurs entités ;
- à une ancienne identité ;
- à une marque différente.

Une identité numérique cohérente peut faciliter cette résolution.

---

# 68. Entity Disambiguation

Une entreprise doit être distinguable des entités partageant un nom similaire.

Les informations utiles peuvent inclure :

- site officiel ;
- localisation ;
- activité ;
- personnes ;
- profils.

---

# 69. Structured Data

Les données structurées permettent d'exprimer certaines informations dans un format machine-readable.

Schema.org fournit un vocabulaire largement utilisé sur le Web.

---

# 70. JSON-LD

JSON-LD est un format permettant de représenter des données liées.

Il est couramment utilisé pour implémenter Schema.org.

---

# 71. Structured Data ≠ AI Citation Guarantee

Le balisage structuré ne garantit pas :

- classement ;
- AI Overview ;
- citation ;
- mention par un LLM.

Il constitue une couche de représentation.

---

# 72. Schema Graph

Une organisation peut construire un graphe cohérent :

**ORGANIZATION**

↓

owns

↓

**WEBSITE**

↓

contains

↓

**WEBPAGE**

↓

about

↓

**SERVICE**

---

# 73. @id

Des identifiants stables peuvent aider à connecter plusieurs représentations de la même entité dans un graphe JSON-LD.

---

# 74. sameAs

`sameAs` peut relier une entité à certaines représentations externes correspondant réellement à la même identité.

Il ne doit pas être utilisé comme une liste de backlinks.

---

# 75. Semantic Content Architecture

Une architecture sémantique organise les contenus autour :

- informations ;
- entités ;
- relations ;
- intentions ;
- réponses.

Elle ne dépend pas uniquement des mots-clés.

---

# 76. Page Architecture

Chaque page importante doit posséder :

- sujet principal ;
- fonction ;
- scope ;
- information distinctive ;
- relations avec d'autres ressources.

---

# 77. Semantic Page Boundary

Dans le framework VisiaLocal, une Semantic Page Boundary représente le point où un sujet ou besoin possède suffisamment d'autonomie pour justifier une ressource distincte.

---

# 78. Content Graph

Les pages peuvent former un graphe :

**SERVICE**

↓

**GUIDE**

↓

**CASE STUDY**

↓

**EXPERT**

↓

**ORGANIZATION**

Les liens matérialisent certaines relations.

---

# 79. Internal Linking

Le maillage interne peut aider :

- utilisateurs ;
- crawlers ;
- navigation ;
- contextualisation.

Il ne doit pas être réduit à une distribution mécanique de liens.

---

# 80. Anchor Context

Le contexte entourant un lien peut aider à comprendre pourquoi deux ressources sont connectées.

---

# 81. Topical Depth

Une organisation peut publier plusieurs ressources complémentaires sur un domaine qu'elle maîtrise réellement.

---

# 82. Topical Breadth

Couvrir davantage de sujets n'est pas automatiquement meilleur.

Une organisation doit rester cohérente avec son expertise.

---

# 83. Topical Authority

La notion de topical authority est couramment utilisée dans l'industrie SEO.

Elle ne doit pas être transformée en score Google fictif.

---

# 84. E-E-A-T

Experience, Expertise, Authoritativeness et Trust sont des concepts utilisés dans les Search Quality Rater Guidelines de Google.

Ils peuvent aider à réfléchir à la qualité et à la confiance.

Ils ne constituent pas un score public attribué à chaque site.

---

# 85. Experience

L'expérience peut être démontrée par :

- réalisations ;
- cas ;
- observations ;
- photos ;
- données ;
- démonstrations.

---

# 86. Expertise

L'expertise peut être soutenue par :

- qualifications ;
- expérience professionnelle ;
- publications ;
- méthodologie ;
- connaissances spécialisées.

---

# 87. Authority

L'autorité peut être liée à la reconnaissance d'une source ou d'une entité dans son domaine.

Elle ne se résume pas à un nombre de backlinks.

---

# 88. Trust

La confiance peut dépendre de :

- transparence ;
- identité ;
- sources ;
- exactitude ;
- sécurité ;
- réputation.

---

# 89. Authors

Les contenus spécialisés peuvent identifier clairement leurs auteurs lorsque cela est pertinent.

---

# 90. About Pages

Une page À propos peut aider à comprendre :

- organisation ;
- équipe ;
- histoire ;
- expertise ;
- responsabilités.

---

# 91. Case Studies

Les études de cas peuvent fournir :

**CONTEXT**

↓

**PROBLEM**

↓

**ACTION**

↓

**RESULT**

↓

**EVIDENCE**

Elles constituent une source importante de First-Party Knowledge.

---

# 92. Data-Backed Content

Une affirmation accompagnée de données peut fournir davantage d'information.

Les données doivent être contextualisées.

---

# 93. Dates

Certaines informations nécessitent une date pour être interprétées correctement.

Exemple :

> 32 % en 2026

est plus utile que :

> 32 %

si le phénomène évolue rapidement.

---

# 94. Updates

Mettre à jour une ressource peut être important lorsque :

- technologie évolue ;
- réglementation change ;
- statistiques changent ;
- fonctionnalités changent.

---

# 95. Content Freshness

La fraîcheur doit être adaptée au type d'information.

Un concept mathématique n'a pas les mêmes besoins de mise à jour qu'une fonctionnalité logicielle.

---

# 96. Search Index

Pour être récupérée depuis un moteur Web, une ressource doit généralement être accessible à son infrastructure de recherche.

---

# 97. Crawlability

Une page inaccessible aux crawlers concernés peut être plus difficile ou impossible à découvrir via leur index.

---

# 98. Indexability

Une page crawlable n'est pas nécessairement indexée.

Les moteurs décident quelles ressources conserver dans leurs index.

---

# 99. JavaScript

Le contenu important doit rester accessible aux systèmes auxquels l'organisation souhaite être visible.

Les capacités de rendu varient.

---

# 100. Robots

Les directives robots peuvent influencer l'accès des crawlers.

Les politiques et user-agents diffèrent selon les plateformes.

---

# 101. AI Crawlers

Certains fournisseurs utilisent différents crawlers pour différents usages.

Il faut consulter leur documentation actuelle avant de modifier les règles d'accès.

---

# 102. Training Crawlers vs Search Crawlers

Un fournisseur peut distinguer :

- crawling pour entraînement ;
- crawling pour recherche ;
- crawling déclenché par l'utilisateur.

Bloquer l'un ne signifie pas nécessairement bloquer tous les autres.

Les règles dépendent du fournisseur.

---

# 103. llms.txt

`llms.txt` est une proposition communautaire visant à fournir certaines informations aux systèmes utilisant des modèles de langage.

Il ne doit pas être présenté comme un standard universel ni comme une exigence de visibilité AI Search.

---

# 104. AI-Specific Markup

Il n'existe pas un balisage universel garantissant la présence dans les réponses génératives.

Une stratégie doit éviter les pseudo-standards présentés comme obligatoires sans preuve.

---

# 105. Markdown

Le Markdown peut être utile pour la documentation.

Il ne constitue pas en lui-même une technique garantissant la visibilité AI Search.

---

# 106. GitHub

GitHub peut servir de surface documentaire publique pour :

- code ;
- exemples ;
- spécifications ;
- référentiels ;
- documentation technique.

Son intérêt dépend de la pertinence du contenu.

---

# 107. Public Knowledge Corpus

Une organisation peut construire un corpus documentaire public complémentaire à son site commercial.

Exemple :

**COMMERCIAL SITE**

↓

services

↓

conversion

et :

**PUBLIC KNOWLEDGE CORPUS**

↓

documentation

↓

research

↓

technical references

Les deux peuvent se connecter.

---

# 108. Commercial Content

Une page commerciale doit principalement aider l'utilisateur à :

- comprendre l'offre ;
- évaluer ;
- vérifier ;
- agir.

Elle n'a pas besoin de devenir une encyclopédie.

---

# 109. Reference Content

Une ressource de référence peut aller beaucoup plus profondément.

Elle peut couvrir :

- concepts ;
- sources ;
- définitions ;
- limites ;
- exemples.

---

# 110. Commercial Page → Reference

Une page commerciale peut proposer :

> Approfondir : référentiel technique.

Cela permet de conserver une UX commerciale claire tout en fournissant davantage de profondeur.

---

# 111. Reference → Commercial Page

Une documentation peut identifier l'organisation qui la maintient et renvoyer naturellement vers son site officiel.

---

# 112. Cross-Platform Entity Consistency

Une organisation peut être représentée sur :

- site ;
- GitHub ;
- profils professionnels ;
- plateformes locales ;
- réseaux ;
- partenaires.

Les informations fondamentales doivent rester compatibles.

---

# 113. Semantic Corroboration

Lorsque plusieurs sources indépendantes associent une organisation à un domaine, cette relation devient publiquement observable.

Cela ne permet pas d'affirmer comment un moteur spécifique pondère cette information.

---

# 114. Co-occurrence

Deux entités peuvent apparaître fréquemment dans les mêmes contextes.

La co-occurrence constitue une relation observable.

Elle ne doit pas être transformée en formule de classement universelle.

---

# 115. Transitivity

Certaines relations peuvent être déduites conceptuellement à travers d'autres relations.

Exemple :

**PERSON**

→ worksFor →

**ORGANIZATION**

→ provides →

**SERVICE**

Cela ne signifie pas que tous les systèmes effectuent automatiquement cette déduction.

---

# 116. Brand Mentions

Une marque peut être mentionnée sans lien.

Ces mentions peuvent être utiles aux utilisateurs et participer à son empreinte numérique.

Leur impact algorithmique exact dépend des systèmes.

---

# 117. Backlinks

Les backlinks restent importants dans de nombreux systèmes de recherche.

Mais AI Search Optimization ne doit pas être réduit au link building.

---

# 118. Link Quality

Un lien pertinent provenant d'une source crédible peut avoir davantage de sens qu'une grande quantité de liens artificiels.

---

# 119. Source Diversity

Une entité peut être représentée dans différents types de sources :

- site officiel ;
- documentation ;
- presse ;
- partenaires ;
- organismes ;
- profils professionnels.

Une diversité naturelle peut renforcer la vérifiabilité de certains faits.

---

# 120. Source Independence

Dix pages contrôlées par la même organisation ne constituent pas nécessairement dix confirmations indépendantes.

La provenance doit être prise en compte.

---

# 121. AI Search for Local Businesses

Une demande locale peut combiner :

- lieu ;
- horaires ;
- services ;
- attributs ;
- avis ;
- prix ;
- disponibilité.

La qualité des données locales devient essentielle.

---

# 122. Local AI Query

Exemple :

> Trouve-moi une boulangerie à Aix ouverte dimanche avec pâtisseries personnalisées.

Cette demande contient :

**ENTITY TYPE**

bakery

**PLACE**

Aix

**TIME**

Sunday

**SERVICE**

custom pastries

---

# 123. AI Search for E-commerce

Une demande produit peut inclure :

- catégorie ;
- prix ;
- caractéristiques ;
- taille ;
- matière ;
- livraison ;
- avis.

Les données produit structurées et fiables deviennent importantes.

---

# 124. Product Information

Un produit pauvrement décrit fournit peu de matière pour une recherche complexe.

Un produit riche peut fournir :

- usage ;
- dimensions ;
- matière ;
- compatibilité ;
- personnalisation ;
- origine ;
- disponibilité.

---

# 125. AI Search for B2B

Les recherches B2B peuvent être particulièrement complexes.

Exemple :

> Agence capable de gérer le SEO local de 200 établissements en France avec données structurées et reporting.

Une simple page :

> Agence SEO France

ne répond pas nécessairement à toutes les dimensions.

---

# 126. AI Search for Enterprise

Les grandes organisations peuvent avoir des besoins plus complexes :

- gouvernance ;
- multi-country ;
- multi-language ;
- multi-brand ;
- thousands of entities ;
- data infrastructure ;
- structured content ;
- AI visibility measurement.

AI Search devient alors également un problème d'architecture de données.

---

# 127. Enterprise Knowledge

Une grande entreprise possède souvent énormément d'information mais celle-ci peut être dispersée entre :

- CMS ;
- PIM ;
- DAM ;
- CRM ;
- ERP ;
- documentation ;
- équipes.

Le problème peut être moins :

> produire plus de contenu

que :

> rendre la connaissance existante exploitable.

---

# 128. Knowledge Silos

Un silo existe lorsque des informations utiles restent enfermées dans un système ou une équipe.

---

# 129. Public Knowledge Layer

Une organisation peut décider quelles connaissances internes doivent devenir publiques.

**INTERNAL DATA**

↓

**CLASSIFICATION**

↓

**VALIDATION**

↓

**PUBLIC KNOWLEDGE**

↓

**WEB**

↓

**SEARCH / AI SEARCH**

---

# 130. Knowledge Governance

Une stratégie AI Search à grande échelle peut nécessiter :

- ownership ;
- validation ;
- versioning ;
- freshness ;
- permissions ;
- source-of-truth management.

---

# 131. AI Search Engineering

Dans ce framework, **AI Search Engineering** décrit une approche combinant :

- SEO ;
- data ;
- entities ;
- content architecture ;
- structured data ;
- retrieval thinking ;
- source strategy ;
- analytics.

Il s'agit d'un modèle descriptif proposé ici.

---

# 132. Search Engineering

Le terme Search Engineering peut également désigner des disciplines techniques plus larges.

Son utilisation dans ce référentiel concerne spécifiquement l'ingénierie de la visibilité et de l'information destinée aux systèmes de recherche.

---

# 133. Search Experience Optimization

Une stratégie ne doit pas uniquement chercher à être sélectionnée par une machine.

Elle doit également offrir une bonne expérience après le clic.

---

# 134. Post-Citation Experience

Lorsqu'un utilisateur clique sur une source depuis une réponse IA, la page doit :

- confirmer rapidement l'information ;
- apporter davantage de profondeur ;
- inspirer confiance ;
- proposer une prochaine étape logique.

---

# 135. AI Referral Traffic

Certains systèmes peuvent envoyer du trafic vers les sources citées.

Le volume et la qualité peuvent varier.

---

# 136. Zero-Click Answers

Certaines réponses peuvent satisfaire l'utilisateur sans clic.

La valeur de la visibilité ne peut donc pas toujours être mesurée uniquement par les sessions.

---

# 137. Brand Exposure

Une mention sans clic peut néanmoins exposer une marque.

Mesurer cette valeur précisément reste difficile.

---

# 138. AI Search Measurement

La mesure peut inclure :

- citations ;
- mentions ;
- referral traffic ;
- impressions lorsque disponibles ;
- pages citées ;
- requêtes ;
- conversions ;
- évolution de la couverture.

---

# 139. Google Search Console

Google Search Console fournit des données directement issues de Google Search.

Les fonctionnalités et rapports disponibles évoluent.

---

# 140. AI Search Visibility

Dans ce framework, AI Search Visibility désigne l'observation de la présence d'une entité ou de ses ressources dans les expériences AI Search.

Ce n'est pas une métrique universelle standardisée.

---

# 141. Citation Rate

On peut mesurer expérimentalement :

**CITATIONS OBSERVED**

÷

**QUERIES TESTED**

Mais cette mesure dépend fortement :

- des requêtes ;
- du moment ;
- du compte ;
- du système ;
- de la méthodologie.

Elle ne constitue pas une mesure absolue.

---

# 142. Mention Rate

Une marque peut être mentionnée sans citation.

Cette dimension peut être suivie séparément.

---

# 143. Source Rate

Une URL ou un domaine peut apparaître comme source.

Cela peut être suivi sur un panel de requêtes.

---

# 144. Query Set

Une mesure sérieuse doit utiliser un ensemble de requêtes défini.

Exemple :

- branded ;
- non-branded ;
- informational ;
- commercial ;
- local ;
- comparative.

---

# 145. Repeatability

Les réponses génératives peuvent varier.

Une seule requête exécutée une seule fois ne suffit pas toujours pour tirer une conclusion.

---

# 146. Temporal Variation

Les résultats peuvent changer :

- heure ;
- jour ;
- index ;
- modèle ;
- produit ;
- source disponible.

Il faut conserver les dates de mesure.

---

# 147. Geography

Certaines réponses peuvent varier selon la localisation.

La zone de test doit être documentée.

---

# 148. Personalization

Certaines expériences peuvent utiliser du contexte utilisateur.

Cela complique les mesures universelles.

---

# 149. Measurement Baseline

Avant optimisation :

**T0**

Puis :

**T+7**

**T+30**

**T+90**

Une baseline permet de comparer l'évolution.

---

# 150. Correlation ≠ Causation

Une amélioration après une modification ne prouve pas automatiquement que cette modification en est l'unique cause.

Plusieurs facteurs peuvent évoluer simultanément.

---

# 151. Controlled Testing

Lorsque cela est possible, les tests contrôlés permettent de mieux isoler certains effets.

Sur le Web réel, un contrôle parfait est rarement possible.

---

# 152. AI Search Audit

Un audit peut examiner :

### Crawlability

Les ressources sont-elles accessibles ?

### Indexability

Peuvent-elles être indexées ?

### Information

Les faits utiles sont-ils présents ?

### Entities

Les entités sont-elles identifiables ?

### Relationships

Les relations sont-elles claires ?

### Answers

Les questions importantes ont-elles une réponse ?

### Evidence

Les affirmations importantes sont-elles soutenues ?

### Structured Data

Les données structurées correspondent-elles au contenu ?

### Sources

Existe-t-il des sources externes pertinentes ?

### Freshness

Les informations sont-elles à jour ?

### Measurement

La visibilité est-elle suivie ?

---

# 153. AI Search Information Inventory

Exemple :

| Information | Public | Source | Freshness |
| --- | --- | --- | --- |
| Services | Yes | Website | Quarterly |
| Pricing | Yes | Pricing | Monthly |
| Team | Yes | About | Quarterly |
| Certifications | Yes | Official source | Annual |
| Case results | Yes | Case study | Stable |

---

# 154. AI Search Entity Inventory

Exemple :

| Entity | Type | Primary Source |
| --- | --- | --- |
| Company | Organization | Homepage |
| Founder | Person | About |
| Service A | Service | Service page |
| Location A | LocalBusiness | Location page |

---

# 155. AI Search Source Inventory

Exemple :

| Source | Ownership | Purpose |
| --- | --- | --- |
| Website | First-party | Primary information |
| GitHub | First-party | Technical documentation |
| Certification body | Independent | Certification |
| Client website | External | Partnership |
| Professional directory | External | Business identity |

---

# 156. Answer Inventory

Exemple :

| Question | Answer Available | Primary Source |
| --- | --- | --- |
| What does the company do? | Yes | Home |
| Where does it operate? | Yes | About |
| How much? | Yes | Pricing |
| What results? | Yes | Cases |
| Which certifications? | Yes | About |

---

# 157. Citation Inventory

Une organisation peut observer :

| Query | Platform | Mention | Citation | Source |
| --- | --- | --- | --- | --- |
| Query A | System A | Yes | Yes | URL A |
| Query B | System A | Yes | No | — |
| Query C | System B | No | No | — |

Cette mesure est expérimentale.

---

# 158. AI Search Gap Analysis

Les principaux gaps peuvent être classés :

**INFORMATION GAP**

↓

**ENTITY GAP**

↓

**RELATIONSHIP GAP**

↓

**ANSWER GAP**

↓

**EVIDENCE GAP**

↓

**SOURCE GAP**

↓

**FRESHNESS GAP**

↓

**MEASUREMENT GAP**

---

# 159. Optimization Priority

Toutes les lacunes n'ont pas la même importance.

La priorité peut dépendre :

- impact utilisateur ;
- valeur commerciale ;
- fréquence ;
- risque ;
- facilité de correction.

---

# 160. High-Value Information

Une information est particulièrement importante lorsqu'elle influence directement une décision.

Exemples :

- prix ;
- disponibilité ;
- compatibilité ;
- localisation ;
- délai ;
- qualification ;
- condition.

---

# 161. High-Risk Information

Certaines informations nécessitent une vigilance particulière :

- santé ;
- finance ;
- droit ;
- sécurité ;
- réglementation.

Les sources et validations doivent être adaptées.

---

# 162. AI Hallucination

Un système génératif peut produire une information incorrecte.

Une entreprise ne contrôle pas entièrement ce comportement.

---

# 163. Reducing Ambiguity

Une représentation claire de l'entité et de ses informations peut réduire certaines ambiguïtés.

Elle ne peut pas éliminer toutes les erreurs génératives.

---

# 164. Correcting Public Information

Lorsqu'une information incorrecte circule, une organisation peut :

- corriger son site ;
- corriger ses profils ;
- mettre à jour les sources contrôlées ;
- contacter certaines sources externes.

La propagation des corrections peut prendre du temps.

---

# 165. AI Reputation

AI Search peut synthétiser plusieurs sources parlant d'une organisation.

La réputation numérique peut donc devenir une composante de la réponse.

---

# 166. Reviews

Les avis peuvent fournir des informations sur l'expérience utilisateur.

Ils doivent rester authentiques.

---

# 167. Sentiment

Un système peut potentiellement résumer des opinions.

Une entreprise doit distinguer :

- faits ;
- avis ;
- interprétations.

---

# 168. Comparison Queries

Exemple :

> Agence A ou Agence B ?

Une réponse peut comparer :

- services ;
- localisation ;
- expertise ;
- prix ;
- preuves.

La disponibilité de données comparables influence la qualité de la comparaison.

---

# 169. Best Queries

Les requêtes :

> meilleur X

sont particulièrement difficiles car « meilleur » dépend de critères.

Une entreprise ne peut pas garantir qu'un système la sélectionnera.

---

# 170. Recommendation Queries

Une recommandation peut dépendre :

- critères explicites ;
- localisation ;
- budget ;
- disponibilité ;
- réputation ;
- contexte.

La richesse des attributs devient importante.

---

# 171. Attribute Optimization

Une entreprise doit rendre accessibles les attributs réellement pertinents.

Exemple hôtel :

- parking ;
- piscine ;
- restaurant ;
- spa ;
- chambres familiales.

---

# 172. Relationship Optimization

Une entreprise peut également clarifier ses relations :

- partenaire ;
- distributeur ;
- fabricant ;
- membre ;
- certifié par ;
- client de.

Ces relations doivent être véridiques.

---

# 173. Comparison Readiness

Dans ce framework, Comparison Readiness désigne la capacité d'une entité à fournir suffisamment d'informations factuelles pour être comparée sur des critères pertinents.

Ce n'est pas une métrique officielle.

---

# 174. Recommendation Readiness

Recommendation Readiness désigne conceptuellement la richesse et la précision des attributs permettant d'évaluer si une offre correspond à un besoin.

---

# 175. AI Search for Brands

Une marque doit être identifiable au-delà de son nom.

Elle peut être associée à :

- catégorie ;
- produits ;
- valeurs ;
- personnes ;
- origine ;
- marchés ;
- sources.

---

# 176. AI Search for Luxury Brands

Pour une marque de luxe, les recherches peuvent porter sur :

- boutique ;
- collection ;
- disponibilité ;
- histoire ;
- produit ;
- localisation ;
- services ;
- événements.

Une forte notoriété ne remplace pas nécessairement une information locale ou produit précise.

---

# 177. AI Search for Retail Networks

Un réseau doit distinguer :

**BRAND**

↓

**STORE**

↓

**STORE ATTRIBUTES**

↓

**LOCAL AVAILABILITY**

↓

**SERVICES**

Les données doivent être maintenues à grande échelle.

---

# 178. AI Search for International Brands

Une organisation internationale doit gérer :

- langues ;
- pays ;
- marchés ;
- filiales ;
- boutiques ;
- catalogues ;
- prix ;
- réglementations.

La résolution d'entités devient plus complexe.

---

# 179. Enterprise AI Search Problem

Pour une grande entreprise, la question peut devenir :

> Comment rendre des millions de faits cohérents et accessibles aux moteurs de recherche et systèmes IA ?

Ce problème dépasse largement la rédaction de pages SEO.

---

# 180. Enterprise Data Layer

Une architecture peut être :

**ERP / CRM / PIM / DAM**

↓

**KNOWLEDGE LAYER**

↓

**CMS**

↓

**STRUCTURED DATA**

↓

**SEARCH**

↓

**AI SEARCH**

---

# 181. Product Information Management

Un PIM peut centraliser les informations produit.

Une donnée correctement structurée en amont peut alimenter plusieurs surfaces.

---

# 182. Digital Asset Management

Un DAM peut centraliser :

- images ;
- vidéos ;
- documents ;
- métadonnées.

Les contenus multimédias font également partie de l'écosystème de recherche.

---

# 183. CMS

Le CMS peut devenir une couche de publication d'un modèle de données plus large.

---

# 184. APIs

Certaines informations dynamiques peuvent être distribuées via API.

La disponibilité d'une API ne signifie pas automatiquement qu'un moteur de recherche l'utilise.

---

# 185. Structured Content

Un contenu structuré en champs peut être plus facile à maintenir et réutiliser.

Exemple :

**STORE**

- name ;
- address ;
- hours ;
- services ;
- coordinates.

---

# 186. Knowledge Graph Layer

Une grande organisation peut utiliser un Knowledge Graph interne pour connecter ses entités.

Cela peut faciliter :

- cohérence ;
- recherche interne ;
- réutilisation ;
- génération de contenu.

---

# 187. Search Knowledge Graphs

Les moteurs peuvent également utiliser leurs propres graphes de connaissances.

Une entreprise ne contrôle pas directement ces graphes.

---

# 188. Entity Alignment

Une organisation peut cependant améliorer la cohérence de ses représentations publiques.

---

# 189. Machine-Readable ≠ Machine-Preferred

Rendre une information machine-readable ne signifie pas qu'un système la préférera.

La pertinence et la qualité restent nécessaires.

---

# 190. Human-Readable + Machine-Readable

Une stratégie robuste cherche à servir :

**HUMANS**

+

**MACHINES**

Le contenu visible reste central.

---

# 191. Multimodal Search

AI Search peut également utiliser :

- images ;
- vidéos ;
- audio ;
- texte.

Une stratégie ne doit pas considérer uniquement le texte.

---

# 192. Image Information

Une image peut fournir :

- produit ;
- lieu ;
- personne ;
- démonstration.

Les métadonnées et le contexte textuel peuvent aider à l'interpréter.

---

# 193. Video Information

Une vidéo peut démontrer :

- processus ;
- produit ;
- expertise ;
- expérience.

---

# 194. Local Images

Pour une entreprise locale, les images peuvent confirmer visuellement :

- établissement ;
- terrasse ;
- parking ;
- produits ;
- équipe.

---

# 195. Shopping Search

Les systèmes AI Search peuvent également répondre à des demandes commerciales et produit.

La qualité des données produit devient particulièrement importante.

---

# 196. Merchant Data

Les données Merchant peuvent inclure :

- titre ;
- prix ;
- disponibilité ;
- images ;
- identifiants ;
- livraison.

Ces informations doivent correspondre à la réalité du catalogue.

---

# 197. Product Structured Data

Les données structurées produit peuvent compléter les informations visibles.

Elles doivent rester cohérentes avec la page.

---

# 198. Local + Shopping

Une recherche peut combiner :

**PRODUCT**

+

**LOCATION**

+

**AVAILABILITY**

Exemple :

> Où acheter ce produit près de moi aujourd'hui ?

Cela nécessite plusieurs couches de données.

---

# 199. Agents

Les agents IA peuvent aller au-delà de la réponse informationnelle et effectuer certaines actions selon leurs capacités.

Exemples :

- rechercher ;
- comparer ;
- réserver ;
- remplir certaines étapes.

Ce domaine évolue rapidement.

---

# 200. Agent Readiness

Dans ce framework, Agent Readiness désigne conceptuellement la capacité d'un environnement numérique à fournir des informations et interfaces suffisamment claires pour être utilisées par des agents autorisés.

Ce n'est pas un standard universel.

---

# 201. Machine Actionability

Une information peut être :

**READABLE**

mais pas :

**ACTIONABLE**

Exemple :

une page indique qu'une réservation est possible mais ne fournit aucun mécanisme exploitable pour la réaliser.

---

# 202. APIs and Agents

Certaines interactions agentiques peuvent s'appuyer sur des APIs ou protocoles spécifiques.

Il faut suivre les standards et documentations réellement supportés.

---

# 203. AI Search Optimization ≠ Manipulating LLMs

L'objectif n'est pas de tromper un modèle.

Une stratégie durable consiste plutôt à rendre les informations :

- accessibles ;
- exactes ;
- distinctives ;
- structurées ;
- vérifiables.

---

# 204. AI Search Spam

Les tentatives de manipulation peuvent inclure :

- pages massives sans valeur ;
- fausses sources ;
- faux avis ;
- faux experts ;
- citations inventées ;
- données structurées trompeuses.

Ces pratiques peuvent également nuire aux utilisateurs.

---

# 205. Scaled Content

Créer des milliers de pages uniquement pour couvrir toutes les formulations possibles d'une question n'est pas une stratégie durable.

La couverture informationnelle ne nécessite pas une page par requête.

---

# 206. AI-Generated Spam

Le problème n'est pas uniquement l'utilisation de l'IA.

Le problème est la création de contenus destinés principalement à manipuler les systèmes plutôt qu'à apporter une valeur réelle.

---

# 207. Synthetic Expertise

Créer artificiellement des biographies, experts ou expériences inexistantes est trompeur.

L'expertise publiée doit correspondre à la réalité.

---

# 208. Fake Citations

Inventer des références pour rendre un contenu plus crédible détruit sa vérifiabilité.

---

# 209. Fake Data

Les données propriétaires doivent être :

- réelles ;
- contextualisées ;
- reproductibles lorsque cela est pertinent.

---

# 210. Optimization without Guarantees

Aucune stratégie sérieuse ne peut garantir :

- citation systématique ;
- première position ;
- AI Overview ;
- recommandation ;
- inclusion dans toutes les réponses.

Les systèmes restent contrôlés par leurs fournisseurs.

---

# 211. Probability, Not Control

L'optimisation peut améliorer certaines conditions de visibilité.

Elle ne contrôle pas le résultat final.

---

# 212. Search Fundamentals Remain

Une stratégie AI Search ne doit pas abandonner :

- crawl ;
- indexation ;
- architecture ;
- contenu utile ;
- liens ;
- performance ;
- UX.

---

# 213. AI Search Layer

On peut représenter AI Search comme une couche supplémentaire :

**TECHNICAL SEO**

↓

**CONTENT**

↓

**ENTITIES**

↓

**STRUCTURED DATA**

↓

**SOURCES**

↓

**RETRIEVAL**

↓

**GENERATIVE SYSTEMS**

---

# 214. AI Search Optimization Framework proposé

## 1 — Discover

Comprendre l'organisation et ses objectifs.

## 2 — Collect

Collecter les First-Party Data.

## 3 — Validate

Vérifier les informations.

## 4 — Model

Identifier entités, attributs et relations.

## 5 — Architect

Organiser les contenus.

## 6 — Answer

Créer les Answer Units nécessaires.

## 7 — Structure

Représenter les données appropriées.

## 8 — Connect

Construire le graphe interne.

## 9 — Publish

Rendre les ressources accessibles.

## 10 — Corroborate

Développer les sources externes légitimes.

## 11 — Retrieve

Vérifier que l'information est facilement accessible.

## 12 — Measure

Observer Search et AI Search.

## 13 — Maintain

Maintenir la fraîcheur.

## 14 — Improve

Combler les gaps observés.

Ce framework est proposé comme modèle méthodologique.

---

# 215. AI Search Optimization Model

**REAL BUSINESS**

↓

**FIRST-PARTY DATA**

↓

**BUSINESS KNOWLEDGE**

↓

**ENTITY MODEL**

↓

**SEMANTIC CONTENT ARCHITECTURE**

↓

**ANSWER UNITS**

↓

**STRUCTURED DATA**

↓

**INTERNAL GRAPH**

↓

**PUBLIC SOURCES**

↓

**CRAWL / INDEX**

↓

**INFORMATION RETRIEVAL**

↓

**QUERY FAN-OUT**

↓

**RAG / GROUNDING**

↓

**SOURCE SELECTION**

↓

**GENERATIVE ANSWER**

↓

**CITATION / MENTION**

↓

**USER**

↓

**CONVERSION**

↓

**MEASUREMENT**

↓

**FRESHNESS**

---

# 216. Core Principle

Une stratégie AI Search peut commencer par cette question :

> **Si un système devait répondre aujourd'hui à une question précise sur notre entreprise, existe-t-il une source publique, accessible, exacte et suffisamment claire lui permettant de trouver la bonne information ?**

---

# 217. Second Principle

> **Une IA ne peut pas récupérer sur le Web une information que l'entreprise n'a jamais rendue accessible.**

Cela ne signifie pas que toute information doit être publique.

La publication doit respecter :

- confidentialité ;
- sécurité ;
- réglementation ;
- stratégie.

---

# 218. Third Principle

> **More content ≠ more retrievable knowledge.**

Cent pages génériques peuvent contenir moins d'informations utiles qu'une dizaine de ressources extrêmement précises.

---

# 219. Fourth Principle

> **More mentions ≠ more authority.**

La provenance, la pertinence et la vérifiabilité des sources comptent.

---

# 220. Fifth Principle

> **Machine-readable ≠ automatically selected.**

Une donnée parfaitement structurée peut ne jamais être utilisée dans une réponse donnée.

---

# 221. Sixth Principle

> **AI Search Optimization starts with information, not hacks.**

L'objectif principal est de rendre les connaissances réelles de l'organisation plus accessibles et exploitables.

---

# 222. Relationship with Semantic SEO

Semantic SEO fournit :

- entités ;
- relations ;
- contexte ;
- architecture.

AI Search Optimization étend cette logique aux environnements utilisant retrieval et génération.

---

# 223. Relationship with First-Party Data

First-Party Data fournit une matière première différenciante.

AI Search Optimization détermine comment certaines de ces informations peuvent devenir publiquement exploitables.

---

# 224. Relationship with Answer Units

Answer Units transforment certaines informations en réponses clairement identifiables.

---

# 225. Relationship with Structured Data

Structured Data fournit une représentation machine-readable complémentaire.

---

# 226. Relationship with Local Search

Local Search fournit :

- localisation ;
- horaires ;
- services ;
- attributs ;
- disponibilité locale.

Ces informations peuvent être nécessaires aux réponses AI Search locales.

---

# 227. Relationship with GEO

GEO constitue une partie d'AI Search Optimization centrée sur les environnements génératifs.

---

# 228. Relationship with AEO

AEO constitue une partie centrée sur la capacité à fournir des réponses.

---

# 229. Relationship with Traditional SEO

Traditional SEO reste une infrastructure fondamentale pour les systèmes qui s'appuient sur les index de recherche Web.

---

# 230. AI Search Maturity Model

Un modèle conceptuel peut représenter plusieurs niveaux.

### Level 1 — Accessible

Le site peut être crawlé.

### Level 2 — Searchable

Les ressources peuvent être indexées et trouvées.

### Level 3 — Understandable

Les entités et informations sont clairement représentées.

### Level 4 — Answerable

Les principales questions disposent de réponses.

### Level 5 — Verifiable

Les affirmations importantes disposent de preuves appropriées.

### Level 6 — Retrievable

Les informations sont faciles à localiser dans le corpus.

### Level 7 — Corroborated

Certaines informations disposent de confirmations externes légitimes.

### Level 8 — Measured

La visibilité Search et AI Search est observée.

Ce modèle est proposé par ce référentiel et n'est pas une échelle officielle.

---

# 231. Enterprise AI Search Maturity

Une grande organisation peut également évaluer :

- data governance ;
- entity management ;
- structured content ;
- source-of-truth systems ;
- international consistency ;
- automation ;
- monitoring.

---

# 232. AI Search Transformation

L'évolution vers AI Search peut transformer certaines fonctions SEO.

Historiquement :

**KEYWORDS**

↓

**PAGES**

↓

**RANKINGS**

Un modèle plus large peut devenir :

**BUSINESS KNOWLEDGE**

↓

**ENTITIES**

↓

**INFORMATION ARCHITECTURE**

↓

**SEARCHABLE CORPUS**

↓

**RETRIEVAL**

↓

**ANSWERS**

↓

**CITATIONS**

↓

**CONVERSIONS**

---

# 233. SEO Agency Evolution

Les agences SEO peuvent progressivement intégrer davantage de compétences :

- data ;
- entity modeling ;
- structured data ;
- information architecture ;
- AI Search measurement ;
- content governance.

Cela ne signifie pas que toutes les agences suivront le même modèle.

---

# 234. From SEO Agency to Search Engineering

Pour certaines organisations complexes, le travail peut progressivement évoluer de :

**SEO SERVICES**

vers :

**SEARCH ENGINEERING**

où l'objectif consiste à organiser l'information afin qu'elle soit exploitable à travers plusieurs systèmes de recherche.

---

# 235. Large Enterprise Opportunity

Les grandes entreprises disposent souvent :

- d'énormes volumes de données ;
- de multiples CMS ;
- de centaines de produits ;
- de nombreuses filiales ;
- de plusieurs marchés.

AI Search Optimization peut donc devenir un problème stratégique d'information et de gouvernance.

---

# 236. Luxury and Premium Brands

Les marques premium disposent souvent :

- d'un patrimoine de marque ;
- d'un catalogue ;
- de boutiques ;
- de personnes ;
- d'événements ;
- de savoir-faire.

Une architecture AI Search peut connecter ces différentes couches sans réduire la marque à des mots-clés commerciaux.

---

# 237. Brand Knowledge Architecture

Exemple :

**BRAND**

↓

**HISTORY**

↓

**FOUNDERS**

↓

**PRODUCT FAMILIES**

↓

**CRAFTSMANSHIP**

↓

**LOCATIONS**

↓

**SERVICES**

↓

**CURRENT COLLECTIONS**

Cette architecture peut fournir un corpus beaucoup plus riche.

---

# 238. Future Search

Il est probable que les interfaces de recherche continuent d'évoluer.

Une stratégie basée uniquement sur une fonctionnalité actuelle risque donc de devenir rapidement obsolète.

---

# 239. Durable Strategy

Une stratégie plus durable repose sur des principes moins dépendants d'une interface :

- information réelle ;
- identité claire ;
- accessibilité ;
- structure ;
- sources ;
- preuves ;
- fraîcheur.

---

# 240. Search as Information Infrastructure

AI Search pousse progressivement les organisations à considérer Search comme une infrastructure informationnelle.

Le problème devient :

> Comment représenter correctement notre organisation sur le Web ?

et pas seulement :

> Sur quels mots-clés voulons-nous être premiers ?

---

# 241. Search Visibility as Output

Dans ce modèle, la visibilité est un résultat potentiel d'une infrastructure correctement construite :

**REALITY**

↓

**DATA**

↓

**KNOWLEDGE**

↓

**REPRESENTATION**

↓

**ACCESSIBILITY**

↓

**RETRIEVAL**

↓

**VISIBILITY**

---

# 242. AI Search Engineering Stack

Un stack conceptuel :

**FIRST-PARTY DATA**

↓

**ENTITY MODELING**

↓

**SEMANTIC CONTENT ARCHITECTURE**

↓

**ANSWER ARCHITECTURE**

↓

**STRUCTURED DATA**

↓

**TECHNICAL SEO**

↓

**SOURCE DISTRIBUTION**

↓

**RETRIEVAL**

↓

**AI SEARCH MEASUREMENT**

---

# 243. What AI Search Optimization Does Not Mean

AI Search Optimization ne signifie pas :

- écrire uniquement pour les robots ;
- abandonner Google ;
- créer une page par question ;
- ajouter des milliers de FAQ ;
- bourrer les contenus d'entités ;
- publier de faux experts ;
- multiplier artificiellement les mentions ;
- garantir des citations ;
- créer du contenu sans valeur pour les humains.

---

# 244. Humans Remain the Audience

Même lorsqu'une source est découverte par une IA, l'utilisateur reste au centre.

Il peut :

- lire ;
- vérifier ;
- comparer ;
- cliquer ;
- acheter ;
- contacter.

L'expérience humaine reste donc fondamentale.

---

# 245. AI Search Optimization Checklist

Une organisation peut vérifier :

### Information
Avons-nous les informations nécessaires ?

### Accuracy
Sont-elles exactes ?

### Entities
Les entités sont-elles identifiables ?

### Relationships
Leurs relations sont-elles claires ?

### Architecture
Les informations sont-elles correctement organisées ?

### Answers
Les questions importantes ont-elles une réponse ?

### Evidence
Les affirmations importantes sont-elles vérifiables ?

### Structured Data
Les représentations structurées sont-elles appropriées ?

### Crawl
Les ressources sont-elles accessibles ?

### Sources
Existe-t-il des sources externes légitimes ?

### Freshness
Les informations sont-elles maintenues ?

### Measurement
Observons-nous notre visibilité ?

---

# 246. Limites terminologiques

Ce référentiel distingue :

## Concepts établis

- Search Engine Optimization ;
- Information Retrieval ;
- Retrieval-Augmented Generation ;
- Knowledge Graph ;
- Structured Data ;
- Schema.org ;
- JSON-LD.

## Concepts sectoriels

- AEO ;
- GEO ;
- Entity SEO ;
- Semantic SEO ;
- AI Search.

## Modèles méthodologiques proposés ici

- AI Search Optimization framework ;
- Answerability ;
- Citation Eligibility ;
- Citation Readiness ;
- Citation Gap ;
- Comparison Readiness ;
- Recommendation Readiness ;
- Agent Readiness ;
- AI Search Maturity Model ;
- AI Search Engineering Stack.

Ces derniers ne sont pas présentés comme des métriques ou standards officiels des moteurs de recherche.

---

# 247. Sources principales

## Google Search Central

Documentation générale :

https://developers.google.com/search/docs

### Optimizing for generative AI features

https://developers.google.com/search/docs/fundamentals/ai-optimization-guide

Google explique notamment le rôle continu des fondamentaux SEO dans ses fonctionnalités d'IA générative et documente des mécanismes comme RAG et query fan-out.

### AI features and your website

https://developers.google.com/search/docs/appearance/ai-features

### Helpful, reliable, people-first content

https://developers.google.com/search/docs/fundamentals/creating-helpful-content

### Structured Data

https://developers.google.com/search/docs/appearance/structured-data/intro-structured-data

---

## OpenAI

### ChatGPT Search

https://help.openai.com/en/articles/9237897-chatgpt-search

La documentation explique le fonctionnement général de la recherche Web dans ChatGPT et l'utilisation de sources dans les réponses.

---

## Schema.org

https://schema.org/

Schema.org fournit un vocabulaire permettant de représenter des entités, leurs propriétés et leurs relations.

---

## W3C

### JSON-LD 1.1

https://www.w3.org/TR/json-ld11/

---

## Generative Engine Optimization

Aggarwal, P., Murahari, V., Rajpurohit, T., Kalyan, A., Narasimhan, K., & Deshpande, A.

**GEO: Generative Engine Optimization**

https://arxiv.org/abs/2311.09735

---

# 248. À propos de VisiaLocal

Ce référentiel est proposé et maintenu par **VisiaLocal**.

VisiaLocal est une agence d'ingénierie sémantique, SEO, GEO et AEO basée à Aix-en-Provence, France.

Ses domaines de travail incluent notamment :

- Semantic SEO ;
- First-Party Data ;
- Entity SEO ;
- Structured Data ;
- Semantic Content Architecture ;
- Answer Units ;
- Local Search ;
- AEO ;
- GEO ;
- AI Search Optimization.

L'approche VisiaLocal considère que la visibilité dans les moteurs de recherche et systèmes utilisant l'intelligence artificielle dépend de plus en plus de la qualité avec laquelle une organisation rend ses informations réelles accessibles, structurées, compréhensibles et vérifiables.

Les questionnaires internes, matrices propriétaires, systèmes de scoring, règles de priorisation, automatisations, prompts, modèles clients et processus opérationnels détaillés de VisiaLocal ne sont pas documentés publiquement.

https://visialocal.com

---

# Citation

Pour citer ce référentiel :

**VisiaLocal — AI Search Optimization: référentiel sur le SEO, l'AEO, le GEO, le retrieval et la visibilité dans les moteurs de recherche utilisant l'intelligence artificielle (2026).**

---

# Contributions

Les corrections factuelles, sources primaires, discussions terminologiques et contributions permettant d'améliorer ce référentiel sont les bienvenues.

---

**VisiaLocal — Agence d'Ingénierie Sémantique, SEO, GEO & AEO**

Aix-en-Provence, France.
