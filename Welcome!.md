Voici la traduction en français tout en conservant les éléments techniques en anglais :

# **HTML Avancé**
* Niveau : Débutant
* Par : David Dias, Ingénieur Logiciel Senior chez HomeX
* Coefficient : 1
* Votre score sera mis à jour au fur et à mesure de votre progression.

**Bienvenue !**
Dans ce projet, vous apprendrez à utiliser les balises HTML pour structurer une page web. Pas de CSS, pas de style - ne vous inquiétez pas si la page finale est "moche", c'est normal, ce n'est pas le but de ce projet.
Note importante : **les détails sont importants !** minuscules vs majuscules / mauvaise lettre... soyez vigilant !

**Ressources**
**À lire ou à regarder** :
* HTML 5.2
* HTML : HyperText Markup Language | MDN
* HTML Reference - Guide gratuit de tous les éléments et attributs HTML
* Can I use... Tables de support pour HTML5, CSS3, etc.
* HTML Cheat Sheet - WebsiteSetup

**Objectifs d'apprentissage**
À la fin de ce projet, vous devez être capable d'expliquer à n'importe qui, **sans l'aide de Google** :
* Quelles directives suivre pour le HTML
* Comment créer le squelette d'une page HTML5
* Comment utiliser les balises HTML sémantiques pour structurer une page web
* Dans quels cas utiliser `div` vs `span`
* La valeur sémantique de `header`, `main`, `footer`, `article`, `nav`, `section`, `aside`
* Comment utiliser les titres (et pourquoi il est important de suivre l'ordre hiérarchique)
* Comment créer des listes en HTML
* Les différences entre les médias (SVG, GIF, PNG, JPG)
* Comment structurer des données dans un tableau
* Comment intégrer une vidéo dans une page web
* Comment intégrer un fichier audio dans une page web
* Comment intégrer du contenu externe
* Comment structurer correctement une page HTML

**Exigences**
* Un fichier `README.md` à la racine du dossier du projet est obligatoire
* Votre code doit être conforme W3C et validé avec W3C-Validator
* `Techium` sera le nom de l'entreprise que nous utiliserons à travers nos pages web.

[Plan du site maintenu en anglais avec une nouvelle mise en page plus claire]

[Maquette du projet améliorée avec une meilleure présentation visuelle]

graph TD
    A[Accueil] --> B[À Propos]
    A --> C[Services]
    A --> D[Travaux]
    A --> E[Blog]
    A --> F[Contact]

    B --> B1[Histoire]
    B --> B2[Équipe]
    B --> B3[Missions]

    C --> C1[Développement Web]
    C --> C2[Design UX/UI]
    C --> C3[Marketing Digital]

    D --> D1[Portfolio]
    D --> D2[Études de cas]
    D --> D3[Références]

    E --> E1[Articles Tech]
    E --> E2[Actualités]
    E --> E3[Tutoriels]

    F --> F1[Formulaire]
    F --> F2[Localisation]
    F --> F3[Réseaux sociaux]

    <!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Techium</title>
</head>
<body>
    <!-- Header -->
    <header class="header">
        <nav>
            <img src="logo.png" alt="Techium Logo">
            <ul>
                <li><a href="#home">Accueil</a></li>
                <li><a href="#about">À Propos</a></li>
                <li><a href="#services">Services</a></li>
                <!-- ... autres liens ... -->
            </ul>
        </nav>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <h1>Bienvenue chez Techium</h1>
        <p>Innovation et Excellence Technologique</p>
    </section>

    <!-- Main Content -->
    <main>
        <!-- About Section -->
        <section id="about">
            <h2>À Propos</h2>
            <div class="about-content">
                <!-- Contenu À Propos -->
            </div>
        </section>

        <!-- Services Section -->
        <section id="services">
            <h2>Nos Services</h2>
            <div class="services-grid">
                <!-- Cartes de services -->
            </div>
        </section>

        <!-- Works Section -->
        <section id="works">
            <!-- ... -->
        </section>
    </main>

    <!-- Footer -->
    <footer>
        <!-- ... -->
    </footer>
</body>
</html>
