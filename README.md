📡 AfriConnect Summit 2026
Site vitrine de la conférence tech panafricaine

📋 Informations du Projet
Auteur	[ISIAKA_ZAINA_RACHEL]
Classe	[L1 R.T]
Année académique	2025-2026
Date de rendu	[24/07/2026]
Type	Projet d'examen - Développement Web
🎯 Description du Projet
AfriConnect Summit 2026 est un site vitrine complet pour une conférence tech panafricaine fictive. L'événement annuel réunit développeurs, entrepreneurs et investisseurs de tout le continent pour partager, innover et construire l'avenir numérique de l'Afrique.

Le site a été conçu pour être moderne, fluide, responsive et entièrement fonctionnel, dans le style épuré de 2026 avec une typographie expressive, des animations sobres, un mode sombre et une navigation fluide.

📄 Pages du Site
Page	Fichier	Description
Accueil	index.html	Présentation générale, compte à rebours, statistiques, intervenants vedettes et sponsors
Programme	programme.html	Planning détaillé sur 3 jours avec système d'onglets interactifs
Intervenants	intervenants.html	Présentation des 9 intervenants avec filtrage dynamique par thématique
Inscription	contact.html	Formulaire d'inscription complet avec validation, FAQ et carte interactive
🛠️ Technologies Utilisées
Frontend
Technologie	Utilisation
HTML5	Structure sémantique, balises <header>, <nav>, <main>, <section>, <article>, <footer>
CSS3	Flexbox, CSS Grid, Variables CSS, Animations, Transitions, Responsive Design
JavaScript	Manipulation DOM, Gestion d'événements, IntersectionObserver, localStorage, Validation formulaire
Google Fonts	Orbitron (titres) + Inter (corps de texte)
Bootstrap Icons	Bibliothèque d'icônes vectorielles
Outils de Développement
Outil	Utilisation
Git	Versioning du code
GitHub	Hébergement du code source
GitHub Pages	Déploiement du site en production
⚡ Fonctionnalités JavaScript Implémentées
#	Fonctionnalité	Description
1	Dark/Light Mode	Basculement entre les thèmes avec persistance dans localStorage
2	Navbar Dynamique	Changement de fond et d'ombre après 80px de défilement
3	Menu Hamburger	Ouverture/fermeture du menu sur mobile
4	Compte à Rebours	Affichage en temps réel des jours/heures/minutes/secondes jusqu'à la conférence
5	Animations au Scroll	Fade-in, slide-in, zoom-in via IntersectionObserver
6	Compteurs Animés	Incrémentation des statistiques au scroll
7	Onglets Programme	Affichage/masquage des plannings des 3 jours
8	Filtrage Intervenants	Filtrage dynamique des cartes par thématique
9	Validation Formulaire	Contrôle complet avec regex (email, téléphone 8+, message 20+)
10	Retour en Haut	Bouton qui apparaît après 300px de défilement avec animation smooth
11	Année Dynamique	new Date().getFullYear() injecté dans le footer
🎨 Design & Identité Visuelle
Palette de Couleurs
Rôle	Couleur	Code Hex
Primaire	Violet	#6C3CE1
Primaire clair	Violet clair	#8B5CF6
Secondaire	Cyan	#00D4FF
Accent	Or	#F59E0B
Fond clair	Blanc	#F8F9FA
Fond sombre	Noir	#0A0A0F
Texte clair	Noir	#1A1A2E
Texte sombre	Blanc	#FFFFFF
Typographie
Rôle	Police	Utilisation
Titres	Orbitron	H1, H2, H3, logo
Corps	Inter	Paragraphes, textes, navigation
📱 Responsive Design
Le site est entièrement responsive avec 3 points de rupture :

Appareil	Largeur	Breakpoint
Mobile	375px	@media (max-width: 375px)
Tablette	768px	@media (max-width: 768px)
Desktop	1200px+	@media (min-width: 1200px)
📂 Structure du Projet
text
NOM-Prenom-AfriConnectSummit/
│
├── index.html              # Page d'accueil
├── programme.html          # Page Programme
├── intervenants.html       # Page Intervenants
├── contact.html            # Page Inscription & Contact
│
├── css/
│   └── style.css          # Styles CSS complets
│
├── js/
│   └── script.js          # JavaScript vanilla
│
├── images/                # Images du site
│   ├── hero-bg.jpg
│   ├── intervenant1.jpg
│   └── ...
│
└── README.md              # Documentation du projet
🔧 Installation & Utilisation
1. Cloner le dépôt
bash
git clone https://github.com/VOTRE-NOM/NOM-Prenom-AfriConnectSummit.git
2. Ouvrir le projet
Ouvrez simplement le fichier index.html dans votre navigateur préféré.

3. Déploiement
Le site est déployé via GitHub Pages :

text
https://zaina-dev.github.io/ISIAKA-Zaina-AfriConnectSummit/

✅ Contraintes Techniques Respectées
☑ HTML5 sémantique (<header>, <nav>, <main>, <section>, <article>, <footer>)
☑ Un seul fichier CSS externe (css/style.css)
☑ Minimum 8 variables CSS dans :root réellement utilisées
☑ Minimum 3 usages distincts de Flexbox
☑ Minimum 2 usages distincts de CSS Grid
☑ 2 polices Google Fonts (Orbitron + Inter)
☑ Responsive via media queries (375px, 768px, 1200px+)
☑ Bootstrap Icons en CDN
☑ Attributs alt sur toutes les images
☑ Code commenté (HTML, CSS, JavaScript)
☑ Transitions CSS sur tous les éléments interactifs
☑ Palette cohérente (4 couleurs principales + dark mode)
☑ Dark/Light mode avec [data-theme="dark"]
👨‍💻 Fonctionnalités JavaScript Détailées
1. Dark Mode / Light Mode
javascript
// Basculement du thème avec persistance localStorage
const currentTheme = htmlElement.getAttribute('data-theme');
const newTheme = currentTheme === 'dark' ? 'light' : 'dark';
localStorage.setItem('theme', newTheme);
2. Compte à Rebours
javascript
// Mise à jour en temps réel toutes les secondes
setInterval(updateCountdown, 1000);
3. Animations au Scroll
javascript
// IntersectionObserver pour déclencher les animations
const observer = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
        if (entry.isIntersecting) {
            entry.target.classList.add('visible');
        }
    });
});
4. Validation Formulaire
javascript
// Validation complète avec regex
const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
const phoneRegex = /^[0-9]{8,}$/;
