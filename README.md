
### Développeur Senior (15 ans d'expérience) | Spécialiste Écosystème JavaScript & Multiplateforme

Développeur passionné et autonome, j’interviens sur l’ensemble du cycle de vie des applications : du web au mobile, en passant par le desktop et l’e-commerce. Mon objectif est de transformer des architectures et besoins complexes en expériences utilisateurs fluides, robustes et performantes.

---

## 🛠 Compétences & Technologies

*   **Frontend :** React.js (v18 & v19), Next.js, Nuxt.js, TypeScript, Tailwind CSS (v3 & v4), ...
*   **Mobile & Desktop :** Capacitor (Android/iOS), Electron.
*   **Backend & Data/Search :** Python, Supabase (PostgreSQL, Auth, Realtime), Node.js, Jamstack, Elasticsearch, ReactiveSearch, ...
*   **E-commerce & CMS :** Expertise historique et approfondie sur Magento et WordPress.
*   **Outils & Écosystème :** Vite, Progressive Web Apps (PWA), Dexie.js (IndexedDB), Leaflet (Cartographie), Git, ...

---

## 🚀 Projets récents & Architecture (Code Source Privé)

*Note : Les codes sources de ces projets sont propriétaires et hébergés sur des dépôts privés. Les architectures et dépendances ci-dessous décrivent mon savoir-faire technique.*

### 1. Aquariums Manager — Application Cross-Platform Desktop & Mobile
*   **Description :** Une application complète destinée aux aquariophiles permettant le suivi rigoureux, l'analyse et la modélisation graphique des paramètres physico-chimiques de multiples environnements aquatiques.
*   **Architecture & Approche technique :** 
    *   **Desktop :** Conçu avec un socle **Electron** + **Electron-Vite** optimisé, packagé via **Electron-Builder** pour Windows (génération d'installateurs NSIS personnalisés). Persistance locale isolée via `electron-store`.
    *   **Mobile :** Portage et synchronisation native Android à l'aide de **Capacitor CLI** (gestion du système de fichiers natif, notifications locales et dialogues système).
    *   **Interface & Data :** UI dynamique et réactive basée sur **React 19**, **TypeScript** et **Tailwind CSS**. Visualisation de données complexes et graphiques d'évolution via **Recharts**. Internationalisation complète intégrée avec `i18next`.
*   **Technologies clés :** `React 19`, `TypeScript`, `Electron 39`, `Capacitor 8`, `Recharts`, `Tailwind CSS`, `i18next`, `Vite 7`.

### 2. AquaShare — Plateforme Web & Mobile Collaborative (Jamstack)
*   **Description :** Écosystème social et collaboratif axé sur le partage d'informations et la géolocalisation pour les passionnés d'aquariophilie.
*   **Architecture & Approche technique :** 
    *   **Framework & SSR :** Architecture **Next.js (v16)** performante avec rendu côté serveur géré via `@supabase/ssr`.
    *   **Cartographie :** Intégration de cartes interactives dynamiques avec **Leaflet** et **React-Leaflet** pour positionner les données géographiques reçues par le module `@capacitor/geolocation`.
    *   **Mobile & Realtime :** Hub mobile cross-platform (Android/iOS via Capacitor) incluant la gestion des notifications push via **Firebase Messaging**. Persistance et gestion de base de données temps réel gérées par **Supabase**.
*   **Technologies clés :** `Next.js 16`, `React 19`, `Supabase (SSR/JS)`, `Capacitor 8`, `Firebase Messaging`, `Leaflet`, `Material UI 6`.

### 3. Smart Notes PWA & Taskbar Desktop Suite — Gestionnaire de Notes Avancé
*   **Description :** Application de prise de notes enrichie, disponible à la fois sous forme de Progressive Web App (PWA) ultra-rapide et d'application utilitaire discrète logée dans la barre des tâches (Taskbar app).
*   **Architecture & Approche technique :** 
    *   **Éditeur de texte enrichi :** Implémentation d'un éditeur WYSIWYG hautement personnalisable basé sur l'écosystème **Tiptap** (Starter-kit, gestion native des images et de la typographie).
    *   **Expérience Utilisateur (UX) :** Organisation des notes par glisser-déposer (*Drag and Drop*) fluide avec `@hello-pangea/dnd`.
    *   **Multi-format :** Version Web configurée en **PWA autonome** (Vite-plugin-pwa) avec synchronisation cloud via **Supabase**. Version Desktop encapsulée dans une fenêtre Electron optimisée pour s'exécuter en arrière-plan depuis la barre des tâches Windows.
*   **Technologies clés :** `React 19`, `Tiptap Suite`, `Vite 7`, `Supabase`, `Vite-plugin-pwa`, `Electron`, `@hello-pangea/dnd`.

### 4. Fidelity App — Solution Mobile de Scan & Fidélité Client
*   **Description :** Application mobile hybride légère permettant de numériser, stocker et générer des cartes de fidélité ou des coupons via des technologies de codes-barres et QR codes.
*   **Architecture & Approche technique :** 
    *   **Matériel natif :** Utilisation intensive des caméras smartphones à travers les modules de scan natifs de Capacitor (`@capacitor-community/barcode-scanner`).
    *   **Génération dynamique :** Moteur de rendu de QR Codes à la volée côté client via `qrcode.react`.
    *   **Routage & Design :** Navigation fluide assurée par `react-router-dom (v7)` et intégration graphique épurée propulsée par le tout nouveau compilateur **Tailwind CSS v4**.
*   **Technologies clés :** `React 19`, `Capacitor 8 (Barcode Scanner)`, `Supabase`, `Tailwind CSS v4`, `React Router 7`.

### 5. WorldCup 2026 — Hub de Suivi & Visualisation de Flux (Realtime)
*   **Description :** Application web de visualisation de tableaux, de statistiques et d'arbres de flux interactifs en temps réel pour la Coupe du Monde de Football.
*   **Architecture & Approche technique :** 
    *   **Visualisation nodale :** Utilisation avancée de **@xyflow/react** (React Flow) pour cartographier et animer dynamiquement les arbres de qualifications et de phases finales sous forme de graphiques nodaux interactifs.
    *   **Data & State :** Agrégation de données distantes via `node-fetch`, synchronisation en temps réel via les primitives de souscription **Supabase** et notifications toast non bloquantes (`react-hot-toast`).
*   **Technologies clés :** `React 19`, `TypeScript`, `@xyflow/react`, `Supabase`, `Tailwind CSS v4 (@tailwindcss/vite)`.

### 6. Hunting Map — Cartographie Interactive Hors-Ligne
*   **Description :** Outil cartographique d'analyse géographique et topographique haute performance, optimisé pour les zones à faible couverture réseau.
*   **Architecture & Approche technique :** 
    *   **Offline-First :** Intégration de **Dexie.js** pour piloter efficacement IndexedDB en tâche de fond, permettant la mise en cache locale de structures de données géographiques lourdes.
    *   **Analyse spatiale :** Exploitation de **Leaflet** poussée avec des extensions complexes de clustering de points (`leaflet.markercluster`) et de cartes de chaleur thermiques (`leaflet.heat`) couplées à un géocodeur d'adresses.
*   **Technologies clés :** `React 19`, `Leaflet`, `React-Leaflet`, `Dexie.js (IndexedDB)`, `Leaflet.heat`, `Vite-plugin-pwa`.

### 7. Family Movies — Plateforme Privée de Préservation d’Archives
*   **Description :** Application web sécurisée et mobile-responsive conçue pour héberger, visionner et préserver des bobines de films familiaux (formats historiques 8mm) numérisés au format MP4.
*   **Architecture & Approche technique :** 
    *   **Performance & PWA :** Optimisation stricte des lecteurs vidéo pour supports mobiles afin d'éviter tout scintillement ou bug d'affichage vertical. Configurée comme une **PWA** hautement sécurisée pour un accès instantané type "App native" par les membres de la famille.
*   **Technologies clés :** `React 18`, `TypeScript`, `Tailwind CSS`, `Vite-plugin-pwa`.

---

## 📫 Me contacter

*   **LinkedIn :** [https://www.linkedin.com/in/nicolas-de-cook/](https://www.linkedin.com/in/nicolas-de-cook/)
*   **Email :** nicolasdecook@gmail.com
