# Brief Senior Product Manager freelance

*Neginvest · 25 novembre 2026 · Contact : Matthieu Hélary, Directeur Product, Tech, Data & IA*

> **En bref**
>
> - **Mission** : Senior Product Manager freelance, contrat de 6 mois jusqu'à fin juin 2027.
> - **Objectif** : une plateforme e-commerce Medusa prête à porter nos 20+ sites B2B, où migrer un site revient à un thème et un plan de redirections.
> - **Vous** : PM ayant déjà mené des refontes e-commerce, à l'aise en engineering, design, product et stakeholder management.
> - **Lieu** : remote friendly, idéalement basé à Lille, présence régulière à Wasquehal.

---

## 1. L'entreprise

Neginvest est une holding française qui construit et opère un portefeuille de plus de 20 marques B2B spécialisées : mobilier de bureau, équipement d'entrepôt et industriel, signalétique et parking. Parmi elles : [Gosto.com](https://www.gosto.com/), [Manulevage](https://www.manulevage.fr/), [Panostock](https://www.panostock.fr/).

Le groupe vend exclusivement aux professionnels. Il est présent en France, en Espagne et au Portugal, s'apprête à lancer l'Italie et veut continuer à s'étendre en Europe. Il grandit de façon organique et par acquisitions.

L'équipe Product, Tech, Data & IA construit en ce moment un data warehouse, des agents IA, la plateforme e-commerce multi-pays et les systèmes logistiques. Elle transforme aussi certains outils SaaS : email, téléphone, CRM, emailing, etc.

---

## 2. Mission et problème à résoudre

### Le contexte

Neginvest remplace ses boutiques PrestaShop par une plateforme e-commerce unique sur Medusa, capable de porter plus de 20 sites de marque. Il manque un pilote produit pour transformer ce travail en backlog et en livraisons.

- **Fait** : un nouveau site, créé sur la plateforme. Il prouve que le socle Medusa + Next.js tient en production. Risque faible : pas d'historique SEO à perdre.
- **Janvier 2027** : un site existant, migré depuis PrestaShop. Il doit prouver qu'on sait migrer sans casser le référencement ni la conversion. Risque élevé : URL qui changent, redirections, positions Google et CA organique à protéger.
- **Ensuite** : les autres marques. Il faut prouver qu'une migration devient une routine, pas un projet. Le risque se répète à chaque site si la première migration n'est pas industrialisée.

### Le problème

En janvier 2027, 2 sites tourneront sur la plateforme. Il en reste plus de 18 à migrer : il faut désormais accélérer fortement. **Le but : une plateforme prête fin juin 2027 pour porter tous les sites**, où migrer un site revient à un thème et un plan de redirections, pas à un projet de développement. Pour y arriver en 6 mois : 12 chantiers, en 4 blocs.

**1. Connecter le SI** : les briques du SI

- **PIM** : on passe de 20 catalogues, chacun dans la base de données de son site, à un catalogue unique, activable par site et par pays, servi par API.
- **OMS** : le bon transporteur pour chaque panier, avec son prix et son délai.
- **CMS** : pages et contenus gérés par le marketing, sans développeur.

**2. Espace client** : tout en ligne

- **Compte client** : devis, commandes, suivi, factures et PDF, retours, recommande, alimentés par l'ERP.
- **Grands comptes** : sous-comptes avec rôles acheteur, approbateur et administrateur, plafonds et circuits d'approbation, prix et catalogue par client.
- **Devis en ligne** : le client convertit son devis en commande.

**3. Achats B2B** : les outils d'achat des clients

- **E-procurement et SSO** : punch-out depuis leurs outils d'achat, connexion unique.
- **Paiements** : intégrer nos prestataires de paiement (PSP).

**4. Vendre plus** : plus de conversion

- **IA dans la recherche** : recherche en langage naturel.
- **Recommandations** : sur la fiche produit.
- **Paniers abandonnés** : relance automatique.
- **Plan de marquage** : mesurer tout le parcours.

En socle de tous les sites : un design system industrialisé, bibliothèque versionnée et un thème par marque.

### Votre rôle

Vous êtes le Senior Product Manager du projet : vous décidez quoi construire, dans quel ordre, et vous vérifiez que ce qui sort répond au besoin. Vous parlez la langue de l'équipe technique et pouvez contribuer au code si vous le souhaitez, mais ce n'est pas votre mission principale.

- Terminer avec les équipes PIM et OMS ces deux briques et leurs contrats d'API : ce que Medusa reçoit, sous quel délai, et ce que voit le client quand une brique ne répond pas.
- Choisir le CMS headless (note construire ou acheter) et le brancher.
- Concevoir l'espace client B2B sur les API de l'ERP, et faire améliorer ces API si nécessaire.
- Porter avec le design et la tech l'industrialisation du design system : composants, thème par marque, accessibilité.
- Spécifier le premier raccordement e-procurement d'un grand compte (PunchOut, SSO) et l'intégration des prestataires de paiement.
- Lancer les chantiers « Vendre plus » (recherche IA, recommandations, relance des paniers abandonnés, plan de marquage), chacun avec sa métrique.
- Vérifier chaque migration par les données : vues de réconciliation dans Snowflake pour s'assurer que tous les produits PrestaShop sont en ligne dans Medusa et que tous les contenus ont migré dans le CMS.
- Construire et prioriser le backlog jusqu'à fin juin, et couper ce qui ne tient pas.
- Rédiger les spécifications et critères d'acceptation, puis recetter chaque livraison.
- Tenir le journal des décisions produit et arbitrer entre marques quand leurs besoins divergent.

Hors périmètre : la migration de janvier, le développement et la migration des données produit.

### Organisation

- **Interlocuteur principal** : Matthieu Hélary (product owner).
- **Outils** : Linear (backlog), GitHub (code), Paper (maquettes), Slack (échanges).
- **Rituels** : point hebdomadaire avec le product owner, démo à chaque livraison.

---

## 3. Stack

Le PM n'a pas à maîtriser chaque outil, mais il doit savoir ce que fait chacun et lire leurs données.

- **E-commerce et front** : Medusa, Next.js, Stripe
- **API** : selon la brique, dans Next.js via Supabase, dans Dolibarr, ou avec API Platform
- **ERP** : Dolibarr
- **Intégrations et jobs** : Trigger.dev, Hookdeck
- **Données et analytics** : Snowflake, dbt, PostHog, GA4, Google Tag Manager
- **CRM et relation client** : Attio, Cargo, Intercom, Allo
- **IA et agents** : Claude, MCP, skills, CLI
- **Design** : Figma, Paper
- **Backlog et code** : Linear, GitHub

---

## 4. Hard skills recherchés

### Produit

- **E-commerce B2B** : connaît les parcours B2B : compte société, devis, prix négociés, paiement à terme, recommande. *Preuve : un parcours B2B livré et ses résultats.*
- **SEO de migration** : plan de redirections, recette des URL avant bascule, suivi Search Console et trafic organique, plan d'action si le trafic chute. *Preuve : une migration avec le trafic organique avant et après.*
- **Priorisation et delivery** : tient 6 mois chargés : coupe, séquence, anticipe les dépendances PIM, OMS et ERP. *Preuve : un projet Linear découpé par le candidat.*
- **Spécification exécutable** : tickets avec contexte, critères d'acceptation et commande de test, exécutables par un humain ou un agent. *Preuve : un ticket réel.*
- **Instrumentation et analytics** : explore PostHog, surtout via MCP, pour comprendre le plan de tracking actuel des sites et prendre des décisions fondées sur les données ; fait évoluer ce plan, une métrique par livraison. *Preuve : un plan de tracking qu'il a écrit.*
- **Conversion et expérimentation** : une hypothèse, une métrique principale et un garde-fou par changement ; sait quoi faire quand le trafic manque.
- **Discovery et cadrage** : part du problème client ou commercial, pas de la solution demandée.
- **Données en autonomie** : interroge Snowflake au quotidien et peut soumettre des PR sur notre projet dbt, par exemple des vues de réconciliation qui vérifient que tous les produits PrestaShop sont en ligne dans Medusa et que tous les contenus ont migré dans le CMS. *Preuve : cas pratique.*

### IA et agents

- **Travail avec l'IA, MCP et skills** : travaille chaque jour avec un agent branché sur nos outils (MCP, skills, CLI, API) et vérifie ce qu'il produit. *Preuve : démonstration en direct.*
- **Diffusion dans l'équipe** : forme l'équipe e-commerce à ces usages pour qu'elle accélère elle aussi : serveurs MCP, skills partagés, bonnes pratiques de vérification.
- **Fonctionnalités IA** : recherche en langage naturel et recommandations, avec une évaluation de la qualité. *Preuve : une fonctionnalité IA livrée et sa mesure.*

> À noter : nous avons construit notre propre serveur MCP pour le PIM.

### Engineering

Vous n'êtes pas développeur, et on ne vous le demande pas. Vous comprenez assez l'architecture pour écrire un contrat entre deux briques et estimer ce que coûte une demande. Si vous codez un peu, vous pouvez soumettre des PR : c'est un plus, pas une attente.

- **Plateforme composable : PIM, OMS, CMS, comptes** : sait quelle brique fait foi pour chaque donnée ; spécifie un parcours qui traverse plusieurs briques avec ses cas d'échec ; écrit les notes construire ou acheter. *Preuve : une architecture qu'il a cadrée.*
- **Replatforming et Medusa** : a mené une migration de plateforme ; comprend les modules, workflows et fournisseurs de livraison de Medusa, le rendu serveur et le cache de Next.js. *Preuve : chiffres avant/après d'une migration.*
- **Intégrations par API** : spécifie l'appel à l'API transport de l'OMS (panier et adresse en entrée, transporteurs et prix en sortie) et la lecture des API de l'ERP : temps de réponse, repli, webhooks. Sait tester lui-même une API dans Postman et/ou avec Claude. *Preuve : une spécification d'intégration.*
- **E-procurement, PunchOut et SSO** : connaît cXML et OCI, les bons de commande électroniques, SAML et OpenID Connect. *Preuve : un raccordement spécifié.*

### Design

- **Design system multi-marques** : porte avec le design et la tech une bibliothèque versionnée, un thème par marque issu des tokens, Storybook et des contrôles d'accessibilité ; suit l'adoption. *Preuve : un design system dont il a suivi l'adoption.*
- **Prototypage par l'IA** : utilise MCP pour designer dans Figma ou Paper, génère des variations de composants à partir du design system, et s'en sert pour vendre vite une idée aux parties prenantes ; teste avant de figer. *Preuve : un prototype récent et comment il a fait décider.*
- **Accessibilité et performance** : WCAG 2.2 AA, European Accessibility Act, Core Web Vitals.

---

## 5. Soft skills

- **Parties prenantes** : fait décider la direction générale, le webmarketing, les équipes commerciales, la logistique et les équipes PIM et OMS avec des faits, et sait dire non.
- **Communication écrite et décision** : une note d'une page qui fait décider plutôt qu'une réunion ; une mise à jour hebdomadaire ; présente ses analyses et recommandations dans un artefact Claude.
- **Priorisation et arbitrages** : tranche quand les besoins des marques ou des clients s'opposent, et explique clairement ce qui passe après et pourquoi.
- **Esprit critique face à l'IA** : garde un jugement humain sur les prix, les contenus légaux, les données clients.
- **Ownership et résultat** : se juge sur la plateforme prête fin juin et les chiffres des sites migrés, pas sur les tickets livrés.
- **Curiosité et transmission** : documente ses décisions pour que l'équipe tienne sans lui après la mission.

---

## 6. Modalités

- **Contrat** : 6 mois. Préavis d'un mois si la collaboration ne fonctionne pas.
- **Lieu** : remote friendly, mais idéalement basé à Lille. Des passages fréquents au bureau de Wasquehal (accessible en tram) sont attendus.
- **Déplacements** : possibles à Strasbourg, par exemple 2 jours tous les 2 mois. Les frais de déplacement sont payés en plus du TJM.
- **TJM** : vu le niveau attendu sur les hard skills, ce n'est pas une mission à 400 €/jour. Mais nous ne sommes ni NVIDIA ni Anthropic : n'attendez pas leurs grilles non plus. On en parle.

---

## 7. Candidater

Envoyez un email à [matthieu@neginvest.fr](mailto:matthieu@neginvest.fr) avec exactement cet objet :

`Freelance PM - Prénom NOM`

Par exemple : `Freelance PM - Matthieu HELARY`. Les emails sont triés automatiquement à partir de cet objet.

Dans votre email :

- **Un dépôt GitHub public** de quelque chose que vous avez construit récemment.
- **Votre histoire** : racontez votre parcours et pourquoi vous êtes pertinent pour cette mission. Sentez-vous libre.

Pas de lettre de motivation ni de CV en PDF. Mettez plutôt ces informations dans le README de votre dépôt, en Markdown.

Votre candidature sera lue à la fois par un humain et par une IA.

**Agences et ESN** : vous pouvez candidater, mais pas via un commercial. La personne que vous proposez nous écrit directement, avec son propre travail sur GitHub.

---

**Contact** : Matthieu Hélary · [matthieu@neginvest.fr](mailto:matthieu@neginvest.fr)
