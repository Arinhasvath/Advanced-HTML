# TASK 0: Create your first webpage

## Objectif
Créer un fichier HTML minimal avec la déclaration DOCTYPE et l'élément HTML de base.

## Étapes détaillées
1. Créer un répertoire `html_advanced` dans `holbertonschool-web_front_end`
2. Créer le fichier `0-index.html` dans ce répertoire

## Code requis
```html
<!DOCTYPE html>
<html lang="en" dir="ltr">
</html>
```

## Explications
- `<!DOCTYPE html>` : Déclare que c'est un document HTML5
- `lang="en"` : Spécifie que le contenu est en anglais
- `dir="ltr"` : Indique que le texte va de gauche à droite (left-to-right)

## Points de vérification
- DOCTYPE en première ligne exactement comme montré
- Balise HTML avec les attributs exacts
- Pas de commentaires ni d'autres éléments
- La page doit être blanche à l'affichage

---

# TASK 1: Structure your webpage

## Objectif
Ajouter les sections principales head et body à la structure HTML.

## Étapes détaillées
1. Copier le contenu de 0-index.html vers 1-index.html
2. Ajouter les balises head et body vides à l'intérieur de html

## Code requis
```html
<!DOCTYPE html>
<html lang="en" dir="ltr">
    <head>
    </head>
    <body>
    </body>
</html>
```

## Explications
- `<head>` : Contient les métadonnées et liens vers ressources externes
- `<body>` : Contient le contenu visible de la page
- L'indentation est importante pour la lisibilité

## Points de vérification
- Structure identique à 0-index.html avec head et body ajoutés
- Les balises head et body doivent être vides
- Respecter l'ordre : head puis body

---

# TASK 2: The head - meta charset, viewport, title, description, favicons

## Objectif
Ajouter les métadonnées essentielles et les liens vers les favicons dans la section head.

## Étapes détaillées
1. Copier le contenu de 1-index.html vers 2-index.html
2. Ajouter dans le head :
   - Charset UTF-8
   - Viewport pour responsive design
   - Titre de la page
   - Description
   - Liens vers favicons

## Code requis
```html
<!DOCTYPE html>
<html lang="en" dir="ltr">
    <head>
        <meta charset="utf-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0, viewport-fit=cover">
        <title>Homepage - Techium</title>
        <meta name="description" content="Techium is a digital agency">
        <link rel="icon" type="image/x-icon" href="./favicon.ico">
        <link rel="icon" type="image/png" href="./favicon.png">
    </head>
    <body>
    </body>
</html>
```

## Explications
- `charset="utf-8"` : Permet l'affichage correct des caractères spéciaux
- `viewport` : Optimise l'affichage sur mobile
- `title` : Titre affiché dans l'onglet du navigateur
- `description` : Description pour les moteurs de recherche
- Deux formats de favicon pour compatibilité maximale

## Points de vérification
- Toutes les balises meta avec attributs exacts
- Ordre des éléments respecté
- Syntaxe correcte des liens favicon

---

# TASK 3: Simple header, main, footer

## Objectif
Ajouter la structure de base d'une page web avec header, main et footer.

## Étapes détaillées
1. Copier le contenu de 2-index.html vers 3-index.html
2. Dans le body, ajouter :
   - Un header avec le texte "Header"
   - Une section main avec "Main content"
   - Un footer avec "Footer"

## Code requis
```html
<!DOCTYPE html>
<html lang="en" dir="ltr">
    <head>
        <!-- Même contenu que 2-index.html -->
    </head>
    <body>
        <header>
            Header
        </header>
        <main>
            Main content
        </main>
        <footer>
            Footer
        </footer>
    </body>
</html>
```

## Explications
- `<header>` : En-tête de la page contenant généralement logo et navigation
- `<main>` : Contenu principal unique à chaque page
- `<footer>` : Pied de page avec informations communes

## Points de vérification
- Structure sémantique correcte
- Textes exactement comme spécifié
- Une seule balise de chaque type

# TÂCHE 4 : Aside

## Ce qu'il faut faire exactement :
1. Créer un nouveau fichier :
```bash
touch article.html
```

2. Copier la base de la tâche 3 mais avec ces changements :
```html
<!DOCTYPE html>
<html lang="en" dir="ltr">
    <head>
        <!-- Même head MAIS changer le title en : -->
        <title>Article - Techium</title>
        <!-- Reste du head identique -->
    </head>
    <body>
        <header>
            Header
        </header>
        <main>
            Main content
            <aside>
                Aside
            </aside>
        </main>
        <footer>
            Footer
        </footer>
    </body>
</html>
```

## Explications très simples :
- `<aside>` : C'est comme une note dans la marge d'un livre
- On le met DANS le `<main>` mais après "Main content"
- Le titre de la page change pour "Article - Techium"

## Vérification :
- Vous devez voir :
  * "Header" en haut
  * "Main content" 
  * "Aside" juste après
  * "Footer" en bas
- 8 espaces avant `<aside>`

---

# TÂCHE 5 : Sections

## Ce qu'il faut faire exactement :
1. Créer nouveau fichier :
```bash
cp 3-index.html 5-index.html
```

2. Dans le `<main>`, remplacer "Main content" par 7 sections :
```html
<main>
    <section>Hero section</section>
    <section>Services section</section>
    <section>Works section</section>
    <section>About section</section>
    <section>Latest news section</section>
    <section>Testimonials section</section>
    <section>Contact section</section>
</main>
```

## Explications très simples :
- `<section>` : C'est comme un chapitre dans un livre
- Chaque section a son propre texte qui dit ce qu'elle est
- L'ordre est TRÈS important
- Toutes les sections sont au même niveau dans `<main>`

## Vérification :
- Vous devez voir 9 lignes de texte :
  * "Header"
  * Les 7 sections dans l'ordre exact
  * "Footer"
- 8 espaces avant chaque `<section>`

---

# TÂCHE 6 : Articles

## Ce qu'il faut faire exactement :
1. Copier le fichier :
```bash
cp 5-index.html 6-index.html
```

2. Ajouter des articles dans 3 sections spécifiques :
```html
<main>
    <section>Hero section</section>
    <section>Services section</section>
    <section>
        Works section
        <article>Work 1</article>
        <article>Work 2</article>
        <article>Work 3</article>
    </section>
    <section>About section</section>
    <section>
        Latest news section
        <article>Article 1</article>
        <article>Article 2</article>
        <article>Article 3</article>
    </section>
    <section>
        Testimonials section
        <article>Testimonial 1</article>
        <article>Testimonial 2</article>
        <article>Testimonial 3</article>
    </section>
    <section>Contact section</section>
</main>
```

## Explications très simples :
- `<article>` : C'est comme un sous-chapitre ou un article de journal
- On ajoute 3 articles dans :
  * La section "Works"
  * La section "Latest news"
  * La section "Testimonials"
- Le reste ne change pas

## Vérification :
- Les articles doivent être exactement dans ces 3 sections
- 12 espaces avant chaque `<article>`
- Les textes doivent être exactement comme montré
- L'ordre est important

---

# TÂCHE 7 : Navigation

## Ce qu'il faut faire exactement :
1. Copier le fichier :
```bash
cp 6-index.html 7-index.html
```

2. Ajouter une navigation dans le header :
```html
<header>
    <nav></nav>
</header>
```

## Explications très simples :
- `<nav>` : C'est le menu de navigation de votre site
- Il doit être VIDE pour l'instant
- Il remplace le texte "Header"
- Il va dans le header mais pas à la fin

## Vérification :
- Le texte "Header" disparaît
- `<nav>` doit être dans `<header>`
- `<nav>` doit être vide
- 12 espaces avant `<nav>`

# TÂCHE 8 : Titre principal Level 1

## Ce qu'il faut faire exactement :
1. Copier le fichier :
```bash
cp 7-index.html 8-index.html
```

2. Ajouter un titre h1 dans main :
```html
<main>
    <h1>Homepage</h1>
    <!-- Garder toutes les sections comme avant -->
</main>
```

## Explications très simples :
- `<h1>` : C'est le titre le plus important de la page
- Il doit être mis AVANT toutes les sections
- Il doit contenir exactement le texte "Homepage"
- Ne touchez pas au reste du code

## Vérification :
- "Homepage" doit apparaître en gros au début du main
- 8 espaces avant le `<h1>`
- Tout le reste doit rester pareil

---

# TÂCHE 9 : Titres Level 2

## Ce qu'il faut faire exactement :
1. Copier le fichier :
```bash
cp 8-index.html 9-index.html
```

2. Ajouter des titres h2 dans chaque section :
```html
<main>
    <h1>Homepage</h1>
    <section>
        <h2>We help you build your brand!</h2>
    </section>
    <section>
        <h2>Services</h2>
    </section>
    <section>
        <h2>Works</h2>
        <article>Work 1</article>
        <article>Work 2</article>
        <article>Work 3</article>
    </section>
    <section>
        <h2>About Us</h2>
    </section>
    <section>
        <h2>Latest news</h2>
        <article>Article 1</article>
        <article>Article 2</article>
        <article>Article 3</article>
    </section>
    <section>
        <h2>Testimonials</h2>
        <article>Testimonial 1</article>
        <article>Testimonial 2</article>
        <article>Testimonial 3</article>
    </section>
    <section>
        <h2>Contact</h2>
    </section>
</main>
```

## Explications très simples :
- `<h2>` : Ce sont les sous-titres principaux
- Chaque section doit avoir son titre h2
- Les textes des titres sont différents pour chaque section
- Les articles restent comme avant

## Vérification :
- Toutes les sections doivent avoir un h2
- Les textes doivent être exactement comme indiqué
- 12 espaces avant chaque `<h2>`
- Articles et leur contenu ne changent pas

---

# TÂCHE 10 : Titres Level 3

## Ce qu'il faut faire exactement :
1. Copier le fichier :
```bash
cp 9-index.html 10-index.html
```

2. Ajouter des titres h3 dans certaines sections :

Dans la section Services :
```html
<section>
    <h2>Services</h2>
    <h3>Design & Concept</h3>
    <h3>Digital Strategy</h3>
    <h3>Content Strategy</h3>
    <h3>UX Design</h3>
    <h3>Web Development</h3>
    <h3>Social Media</h3>
</section>
```

Dans la section Works (dans chaque article) :
```html
<section>
    <h2>Works</h2>
    <article>
        <h3>Interior Design</h3>
    </article>
    <article>
        <h3>Web Development</h3>
    </article>
    <article>
        <h3>Personal Brand</h3>
    </article>
</section>
```

Dans la section About Us :
```html
<section>
    <h2>About Us</h2>
    <h3>Who are we</h3>
    <h3>Our culture</h3>
    <h3>How we work</h3>
</section>
```

Dans la section Latest news (dans chaque article) :
```html
<section>
    <h2>Latest news</h2>
    <article>
        <h3>Hoc loco tenere se Triarius non potuit.</h3>
    </article>
    <article>
        <h3>Ut alios omittam, hunc appello, quem ille unum secutus est.</h3>
    </article>
    <article>
        <h3>Bestiarum vero nullum iudicium puto.</h3>
    </article>
</section>
```

## Explications très simples :
- `<h3>` : Ce sont les sous-sous-titres
- Ils vont dans 4 sections spécifiques :
  * Services (6 h3)
  * Works (3 h3 dans les articles)
  * About Us (3 h3)
  * Latest news (3 h3 dans les articles)
- Les textes doivent être exactement comme montrés
- L'ordre est très important

## Vérification :
- Comptez les h3 dans chaque section
- Vérifiez l'orthographe exacte des textes
- 16 espaces avant les h3 hors articles
- 20 espaces avant les h3 dans les articles

# TÂCHE 11 : StyleGuide

## Ce qu'il faut faire exactement :
1. Créer un nouveau fichier :
```bash
touch 11-styleguide.html
```

2. Créer une nouvelle page avec cette structure :
```html
<!DOCTYPE html>
<html lang="en" dir="ltr">
    <head>
        <meta charset="utf-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0, viewport-fit=cover">
        <title>Styleguide - Techium</title>
        <meta name="description" content="Techium is a digital agency">
        <link rel="icon" type="image/x-icon" href="./favicon.ico">
        <link rel="icon" type="image/png" href="./favicon.png">
    </head>
    <body>
        <header></header>
        <main>
            <section>
                <header>
                    <h2>Headings</h2>
                </header>
                <h1>Heading level 1</h1>
                <h2>Heading level 2</h2>
                <h3>Heading level 3</h3>
                <h4>Heading level 4</h4>
                <h5>Heading level 5</h5>
                <h6>Heading level 6</h6>
            </section>
        </main>
        <footer></footer>
    </body>
</html>
```

## Explications très simples :
- C'est une nouvelle page qui montre tous les styles de titres
- Le titre de la page est "Styleguide - Techium"
- Il y a une section qui contient :
  * Un header avec h2 "Headings"
  * Tous les niveaux de titres de h1 à h6
- Les header et footer sont vides

## Vérification :
- Title doit être exactement "Styleguide - Techium"
- Les textes des titres doivent être exactement comme indiqué
- L'ordre des titres doit être de h1 à h6
- Header et footer doivent être vides

---

# TÂCHE 12 : Paragraphes

## Ce qu'il faut faire exactement :
1. Copier le fichier :
```bash
cp 10-index.html 12-index.html
```

2. Ajouter des paragraphes dans plusieurs sections.

Dans la section "About Us" :
```html
<section>
    <h2>About Us</h2>
    <h3>Who are we</h3>
    <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ipsum, omnis expedita! Eum, praesentium cumque accusantium rem, sit quaerat est nisi ratione, deserunt ducimus quidem iste dicta quibusdam atque maxime cum!
    </p>
    <h3>Our culture</h3>
    <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ipsum, omnis expedita! Eum, praesentium cumque accusantium rem, sit quaerat est nisi ratione, deserunt ducimus quidem iste dicta quibusdam atque maxime cum!
    </p>
    <h3>How we work</h3>
    <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ipsum, omnis expedita! Eum, praesentium cumque accusantium rem, sit quaerat est nisi ratione, deserunt ducimus quidem iste dicta quibusdam atque maxime cum!
    </p>
</section>
```

Dans la section "Latest news" :
```html
<section>
    <h2>Latest news</h2>
    <article>
        <p>Career</p>
        <h3>Hoc loco tenere se Triarius non potuit.</h3>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Id Sextilius factum negabat. Quo tandem modo? At eum nihili facit; Quae contraria sunt his, malane?</p>
    </article>
    <article>
        <p>Digital Life</p>
        <h3>Ut alios omittam, hunc appello, quem ille unum secutus est.</h3>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Tum mihi Piso: Quid ergo? Tum ille: Ain tandem? Non autem hoc: igitur ne illud quidem. Sed quod proximum fuit non vidit. Nos commodius agimus. An nisi populari fama?</p>
    </article>
    <article>
        <p>Social</p>
        <h3>Bestiarum vero nullum iudicium puto.</h3>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Non igitur bene. Quid enim est a Chrysippo praetermissum in Stoicis? Pugnant Stoici cum Peripateticis. Prioris generis est docilitas, memoria; Apparet statim, quae sint officia, quae actiones.</p>
    </article>
</section>
```

AJOUTER aussi :
- Au début des sections "Services", "Works", "About Us", "Latest news", "Testimonials" et "Contact", ajouter un paragraphe après le h2 :

```html
<section>
    <h2>Services</h2>
    <p>We work with you</p>
    <!-- Reste de la section -->
</section>

<section>
    <h2>Works</h2>
    <p>Take a look in our portfolio</p>
    <!-- Reste de la section -->
</section>

<!-- Etc. pour chaque section avec ces textes :
About Us -> "Everything about us"
Latest news -> pas de paragraphe d'intro
Testimonials -> "We are more than a digital company"
Contact -> "We like to know new people"
-->
```

## Explications très simples :
- Les paragraphes utilisent la balise `<p>`
- Il y a deux types de paragraphes à ajouter :
  1. Les paragraphes d'introduction après les h2
  2. Les paragraphes de contenu dans About Us et Latest News
- Le texte Lorem ipsum doit être exactement comme indiqué
- Les espacements sont importants

## Vérification :
- Tous les textes doivent être exactement comme indiqué
- Les paragraphes d'intro sont après les h2
- Le formatage (espaces) doit être respecté
- Pas de paragraphe d'intro pour Latest news

# TÂCHE 13 : StyleGuide Paragraphes

## Ce qu'il faut faire exactement :
1. Copier le fichier :
```bash
cp 11-styleguide.html 13-styleguide.html
```

2. Ajouter une nouvelle section après celle des headings :
```html
<main>
    <!-- Garder la section headings -->
    <section>
        <header>
            <h2>Paragraph</h2>
        </header>
        <h2>Heading with a subtitle</h2>
        <p>This is my subtitle</p>
        <p>
            Nunc lacinia ante nunc ac lobortis. Interdum adipiscing gravida odio porttitor sem non mi integer non faucibus ornare mi ut ante amet placerat aliquet. Volutpat eu sed ante lacinia sapien lorem accumsan varius montes viverra nibh in adipiscing blandit tempus accumsan.
        </p>
    </section>
</main>
```

## Explications très simples :
- On crée une nouvelle section pour montrer les paragraphes
- Elle contient :
  * Un header avec h2 "Paragraph"
  * Un h2 avec son sous-titre
  * Un long paragraphe exemple
- Le texte doit être copié exactement

## Vérification :
- La section doit venir après celle des headings
- Les textes doivent être identiques à l'exemple
- L'indentation doit être correcte (8 espaces avant section)

---

# TÂCHE 14 : Span

## Ce qu'il faut faire exactement :
1. Copier le fichier :
```bash
cp 12-index.html 14-index.html
```

2. Modifier le header pour ajouter un span :
```html
<header>
    <span>Techium</span>
    <nav></nav>
</header>
```

## Explications très simples :
- `<span>` : C'est pour un petit bout de texte
- Il doit contenir exactement "Techium"
- Il va AVANT la navigation
- La navigation reste vide

## Vérification :
- "Techium" doit apparaître dans le header
- Le span doit être avant nav
- Nav doit rester vide
- 12 espaces avant span

---

# TÂCHE 15 : Div

## Ce qu'il faut faire exactement :
1. Copier le fichier :
```bash
cp 14-index.html 15-index.html
```

2. Entourer des contenus avec des div :

Dans le header :
```html
<header>
    <div>
        <span>Techium</span>
        <nav></nav>
    </div>
</header>
```

Dans le main :
```html
<main>
    <div>
        <section>
            <div>
                <!-- Contenu de la section -->
            </div>
        </section>
        <!-- Répéter pour chaque section -->
    </div>
</main>
```

Dans le footer :
```html
<footer>
    <div>
        <!-- Contenu du footer -->
    </div>
</footer>
```

## Explications très simples :
- `<div>` : C'est une boîte qui groupe des éléments ensemble
- Il faut ajouter des div :
  1. Autour du contenu du header
  2. Autour de toutes les sections dans main
  3. Dans chaque section
  4. Dans le footer
- Le contenu ne change pas, on l'entoure juste

## Vérification :
- Tous les contenus doivent être dans des div
- Les div doivent être correctement imbriqués
- L'indentation doit augmenter de 4 espaces à chaque div
- Le contenu reste le même

---

# TÂCHE 16 : Structure des sections

## Ce qu'il faut faire exactement :
1. Copier le fichier :
```bash
cp 15-index.html 16-index.html
```

2. Réorganiser chaque section avec header et div :
```html
<section>
    <header>
        <h2>Section titre</h2>
        <p>Section paragraphe d'intro</p>
    </header>
    <div>
        <!-- Reste du contenu de la section -->
    </div>
</section>
```

Il faut faire ça pour TOUTES les sections en gardant leur contenu spécifique.

## Explications très simples :
- Chaque section doit avoir :
  1. Un `<header>` qui contient le h2 et le paragraphe d'intro
  2. Un `<div>` qui contient tout le reste
- Le contenu ne change pas, on le réorganise juste
- Faire ça pour toutes les sections

## Vérification :
- Toutes les sections doivent avoir la même structure
- Le contenu de chaque section reste le même
- L'indentation doit être correcte
- Les headers contiennent h2 et paragraphe d'intro

# TÂCHE 17 : Commentaires

## Ce qu'il faut faire exactement :
1. Copier le fichier :
```bash
cp 16-index.html 17-index.html
```

2. Ajouter des commentaires avant chaque section principale :
```html
<body>
    <!-- Header -->
    <header>
        <!-- Contenu du header -->
    </header>

    <!-- Main -->
    <main>
        <!-- Hero section -->
        <section>
            <!-- Contenu hero -->
        </section>

        <!-- Services section -->
        <section>
            <!-- Contenu services -->
        </section>

        <!-- Works section -->
        <section>
            <!-- Contenu works -->
        </section>

        <!-- About Us section -->
        <section>
            <!-- Contenu about -->
        </section>

        <!-- Latest news section -->
        <section>
            <!-- Contenu news -->
        </section>

        <!-- Testimonials section -->
        <section>
            <!-- Contenu testimonials -->
        </section>

        <!-- Contact section -->
        <section>
            <!-- Contenu contact -->
        </section>
    </main>

    <!-- Footer -->
    <footer>
        <!-- Contenu footer -->
    </footer>
</body>
```

## Explications très simples :
- Les commentaires commencent par <!-- et finissent par -->
- Il faut un commentaire :
  * Avant le header
  * Avant le main
  * Avant chaque section
  * Avant le footer
- Les commentaires doivent être exactement comme montrés
- Laisser une ligne vide avant chaque commentaire

## Vérification :
- Tous les commentaires sont présents
- Les textes sont exactement comme indiqué
- L'espacement est correct
- Le reste du code ne change pas

---

# TÂCHE 18 : Lien logo

## Ce qu'il faut faire exactement :
1. Copier le fichier :
```bash
cp 17-index.html 18-index.html
```

2. Modifier le header pour ajouter un lien autour du span :
```html
<header>
    <div>
        <div>
            <a href="/">
                <span>Techium</span>
            </a>
        </div>
        <nav></nav>
    </div>
</header>
```

## Explications très simples :
- `<a href="/">` : Crée un lien vers la page d'accueil
- Il faut :
  1. Ajouter une nouvelle div autour du lien
  2. Mettre le span existant dans le lien
- La navigation reste inchangée

## Vérification :
- Le texte "Techium" doit être cliquable
- href doit être exactement "/"
- L'indentation doit être correcte
- La structure div > div > a > span doit être respectée

---

# TÂCHE 19 : Création de nouvelles pages

## Ce qu'il faut faire exactement :
1. Créer 3 nouveaux fichiers :
```bash
cp 18-index.html about.html
cp 18-index.html latest_news.html
cp 18-index.html contact.html
```

2. Modifier uniquement le titre dans chaque fichier :

Pour about.html :
```html
<head>
    <title>About - Techium</title>
    <!-- Reste du head identique -->
</head>
```

Pour latest_news.html :
```html
<head>
    <title>Latest news - Techium</title>
    <!-- Reste du head identique -->
</head>
```

Pour contact.html :
```html
<head>
    <title>Contact - Techium</title>
    <!-- Reste du head identique -->
</head>
```

## Explications très simples :
- Créer 3 copies exactes de index.html
- Dans chaque copie, changer UNIQUEMENT la balise title
- Le reste du code reste exactement pareil
- Les tirets et majuscules sont importants dans les titres

## Vérification :
- Vous devez avoir 3 nouveaux fichiers
- Seule la balise title change dans chaque fichier
- Les titres doivent être exactement comme indiqué
- Tout le reste du code doit être identique à index.html

# TÂCHE 20 : Ajouter des liens de navigation

## Ce qu'il faut faire exactement :
1. Copier le fichier :
```bash
cp 18-index.html 20-index.html
```

2. Remplir la navigation avec une liste de liens :
```html
<nav>
    <ul>
        <li><a href="/">Home</a></li>
        <li><a href="#services">Services</a></li>
        <li><a href="#works">Works</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#latest_news">Latest news</a></li>
        <li><a href="#testimonials">Testimonials</a></li>
        <li><a href="#contact">Contact</a></li>
    </ul>
</nav>
```

## Explications très simples :
- `<ul>` : C'est une liste non ordonnée
- `<li>` : C'est un élément de la liste
- `#services` : C'est un lien vers une section de la page
- L'ordre des liens est très important
- Le premier lien pointe vers la page d'accueil (/)
- Les autres pointent vers les sections (#nom-section)

## Vérification :
- La nav ne doit contenir qu'une seule liste
- 7 liens exactement
- Les textes doivent être exactement comme indiqués
- Les href doivent être exacts (/ ou #section)
- L'indentation doit être correcte

---

# TÂCHE 21 : Liens sociaux

## Ce qu'il faut faire exactement :
1. Copier le fichier :
```bash
cp 20-index.html 21-index.html
```

2. Ajouter les liens sociaux dans le footer :
```html
<footer>
    <div>
        <ul>
            <li>
                <a href="https://www.facebook.com/HolbertonSchool/">Facebook</a>
            </li>
            <li>
                <a href="https://twitter.com/holbertonschool">Twitter</a>
            </li>
            <li>
                <a href="https://www.instagram.com/holbertonschool/">Instagram</a>
            </li>
        </ul>
    </div>
</footer>
```

## Explications très simples :
- Les liens sociaux vont dans une liste
- Chaque lien doit avoir l'URL exacte
- L'ordre est : Facebook, Twitter, Instagram
- Les URLs doivent être exactement comme montrées
- Les noms des réseaux doivent avoir une majuscule

## Vérification :
- 3 liens exactement
- URLs complètes et exactes
- Textes avec majuscules
- Structure ul > li > a
- L'indentation doit être correcte

---

# TÂCHE 22 : Boutons liens

## Ce qu'il faut faire exactement :
1. Copier le fichier :
```bash
cp 21-index.html 22-index.html
```

2. Ajouter des liens "boutons" dans 3 sections :

Hero section :
```html
<section>
    <div>
        <h2>We help you build your brand!</h2>
        <a href="#">Get started</a>
    </div>
</section>
```

About Us section :
```html
<section>
    <div>
        <h2>About Us</h2>
        <p>Everything about us</p>
        <div>
            <!-- Contenu existant -->
            <a href="about.html">Learn more about us</a>
        </div>
    </div>
</section>
```

Contact section :
```html
<section>
    <div>
        <h2>Contact</h2>
        <p>We like to know new people</p>
        <div>
            <p>Lorem ipsum...</p>
            <a href="contact.html">Get in touch</a>
        </div>
    </div>
</section>
```

## Explications très simples :
- Ajouter 3 nouveaux liens :
  1. "Get started" dans Hero (href="#")
  2. "Learn more about us" dans About (href="about.html")
  3. "Get in touch" dans Contact (href="contact.html")
- La position de chaque lien est importante
- Les textes doivent être exactement comme montrés

## Vérification :
- 3 nouveaux liens dans les bonnes sections
- Textes exactement comme indiqués
- href corrects pour chaque lien
- Position correcte dans chaque section

# TÂCHE 23 : Transformer les h3 en liens

## Ce qu'il faut faire exactement :
1. Copier le fichier :
```bash
cp 22-index.html 23-index.html
```

2. Modifier les h3 dans 3 sections :

Section Services :
```html
<section>
    <div>
        <h3><a href="#">Design & Concept</a></h3>
        <h3><a href="#">Digital Strategy</a></h3>
        <h3><a href="#">Content Strategy</a></h3>
        <h3><a href="#">UX Design</a></h3>
        <h3><a href="#">Web Development</a></h3>
        <h3><a href="#">Social Media</a></h3>
    </div>
</section>
```

Section Works :
```html
<section>
    <div>
        <article>
            <h3><a href="#">Interior Design</a></h3>
        </article>
        <article>
            <h3><a href="#">Web Development</a></h3>
        </article>
        <article>
            <h3><a href="#">Personal Brand</a></h3>
        </article>
    </div>
</section>
```

Section Latest News :
```html
<section>
    <div>
        <article>
            <h3><a href="#">Hoc loco tenere se Triarius non potuit.</a></h3>
        </article>
        <article>
            <h3><a href="#">Ut alios omittam, hunc appello, quem ille unum secutus est.</a></h3>
        </article>
        <article>
            <h3><a href="#">Bestiarum vero nullum iudicium puto.</a></h3>
        </article>
    </div>
</section>
```

## Explications très simples :
- Il faut mettre des liens dans tous les h3 de ces 3 sections
- Les liens pointent vers # (page actuelle)
- Le texte existant du h3 va dans le lien
- La structure doit être h3 > a > texte
- Ne pas toucher aux autres h3

## Vérification :
- Tous les h3 des 3 sections doivent contenir des liens
- href="#" pour tous les liens
- Les textes ne changent pas
- L'indentation doit être correcte

---

# TÂCHE 24 : Liste des liens

## Ce qu'il faut faire exactement :
1. Copier le fichier :
```bash
cp 23-index.html 24-index.html
```

2. Mettre tous les liens de navigation dans des listes :

Navigation principale :
```html
<nav>
    <ul>
        <li><a href="/">Home</a></li>
        <li><a href="#services">Services</a></li>
        <li><a href="#works">Works</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#latest_news">Latest news</a></li>
        <li><a href="#testimonials">Testimonials</a></li>
        <li><a href="#contact">Contact</a></li>
    </ul>
</nav>
```

Liens sociaux dans le footer :
```html
<footer>
    <div>
        <ul>
            <li><a href="https://www.facebook.com/HolbertonSchool/">Facebook</a></li>
            <li><a href="https://twitter.com/holbertonschool">Twitter</a></li>
            <li><a href="https://www.instagram.com/holbertonschool/">Instagram</a></li>
        </ul>
    </div>
</footer>
```

## Explications très simples :
- Tous les liens doivent être dans des `<li>`
- Les `<li>` doivent être dans des `<ul>`
- Ne pas changer les liens eux-mêmes
- Juste ajouter la structure ul/li autour

## Vérification :
- Navigation principale : 7 li dans un ul
- Footer : 3 li dans un ul
- Les liens restent exactement les mêmes
- L'indentation doit être correcte

---

# TÂCHE 25 : Navigation secondaire

## Ce qu'il faut faire exactement :
1. Copier le fichier :
```bash
cp 24-index.html 25-index.html
```

2. Ajouter une navigation secondaire dans le footer :
```html
<footer>
    <div>
        <!-- Liens sociaux existants -->
    </div>
    <div>
        <ul>
            <li><a href="#">Terms of Use</a></li>
            <li><a href="#">Privacy Policy</a></li>
            <li><a href="#">Cookie Policy</a></li>
        </ul>
    </div>
</footer>
```

## Explications très simples :
- Ajouter une nouvelle div dans le footer
- Cette div contient une liste avec 3 liens
- Tous les liens pointent vers # (page actuelle)
- Les textes doivent être exactement comme montrés
- Ne pas toucher aux liens sociaux existants

## Vérification :
- Nouvelle div après celle des liens sociaux
- 3 nouveaux liens exactement
- Textes avec majuscules comme montrés
- href="#" pour tous les nouveaux liens
- Structure ul > li > a respectée

# TÂCHE 26 : Exemples de listes pour le styleguide

## Ce qu'il faut faire exactement :
1. Copier le fichier :
```bash
cp 13-styleguide.html 26-styleguide.html
```

2. Ajouter une nouvelle section pour les listes :
```html
<main>
    <!-- Garder les sections précédentes -->
    <section>
        <header>
            <h2>Lists</h2>
        </header>
        <div>
            <!-- Liste non ordonnée -->
            <h3>Unordered</h3>
            <ul>
                <li>Dolor pulvinar etiam magna etiam.</li>
                <li>Sagittis adipiscing lorem eleifend.</li>
                <li>Felis enim feugiat dolore viverra.</li>
            </ul>

            <!-- Liste ordonnée -->
            <h3>Ordered</h3>
            <ol>
                <li>Dolor pulvinar etiam magna etiam.</li>
                <li>Sagittis adipiscing lorem eleifend.</li>
                <li>Felis enim feugiat dolore viverra.</li>
            </ol>

            <!-- Liste de définitions -->
            <h3>Definition</h3>
            <dl>
                <dt>Definition List title</dt>
                <dd>Definition text.</dd>
                <dt>Startup</dt>
                <dd>A startup company or startup is a company or temporary organization designed to search for a repeatable and scalable business model.</dd>
                <dt>Water</dt>
                <dd>A colorless, transparent, odorless liquid that forms the seas, lakes, rivers, and rain and is the basis of the fluids of living organisms.</dd>
            </dl>
        </div>
    </section>
</main>
```

## Explications très simples :
- Ajouter une nouvelle section après les autres
- Elle montre 3 types de listes :
  1. `<ul>` : liste à puces
  2. `<ol>` : liste numérotée
  3. `<dl>` : liste de définitions avec `<dt>` (terme) et `<dd>` (définition)
- Les textes doivent être exactement comme montrés
- Chaque type de liste a son titre h3

## Vérification :
- La section vient après les sections existantes
- Les 3 types de listes sont présents
- Les textes sont copiés exactement
- L'indentation est correcte

---

# TÂCHE 27 : Ligne horizontale et copyright

## Ce qu'il faut faire exactement :
1. Copier le fichier :
```bash
cp 25-index.html 27-index.html
```

2. Ajouter dans le footer :
```html
<footer>
    <div>
        <!-- Liens sociaux -->
    </div>
    <hr>
    <p>© 2020 Techium, made with ♥ by students at Holberton School.</p>
</footer>
```

## Explications très simples :
- `<hr>` : Crée une ligne horizontale
- Ajouter la ligne après les liens sociaux
- Ajouter le paragraphe de copyright après la ligne
- Le texte doit être exactement comme montré
- Ne pas oublier le symbole © et le ♥

## Vérification :
- HR ajouté au bon endroit
- Paragraphe copyright après HR
- Texte exactement comme montré
- Tous les symboles présents (©, ♥)

---

# TÂCHE 28 : Exemple de ligne horizontale dans le styleguide

## Ce qu'il faut faire exactement :
1. Copier le fichier :
```bash
cp 26-styleguide.html 28-styleguide.html
```

2. Ajouter une nouvelle section :
```html
<section>
    <header>
        <h2>Horizontal rule</h2>
    </header>
    <div>
        <hr>
    </div>
</section>
```

## Explications très simples :
- Ajouter une nouvelle section après la section Lists
- La section montre juste une ligne horizontale
- Structure :
  1. header avec h2 "Horizontal rule"
  2. div contenant un hr
- Garder l'indentation correcte

## Vérification :
- Section après la section Lists
- Titre exact "Horizontal rule"
- HR dans un div
- Structure header > h2 respectée

# TÂCHE 29 : Citations des clients

## Ce qu'il faut faire exactement :
1. Copier le fichier :
```bash
cp 27-index.html 29-index.html
```

2. Modifier la section Testimonials :
```html
<section>
    <header>
        <h2>Testimonials</h2>
        <p>We are more than a digital company</p>
    </header>
    <div>
        <article>
            <blockquote>
                <p>I am completely blown away. Thanks to Techium, we've just launched our 5th website!</p>
                <cite>Yuri Y.</cite>
            </blockquote>
        </article>
        <article>
            <blockquote>
                <p>Thank you so much for your help. Techium company is awesome!</p>
                <cite>Dorrie S.</cite>
            </blockquote>
        </article>
        <article>
            <blockquote>
                <p>I love your system. Definitely worth the investment. I'd be lost without Techium company.</p>
                <cite>Sven H.</cite>
            </blockquote>
        </article>
    </div>
</section>
```

## Explications très simples :
- `<blockquote>` : Pour les citations longues
- `<cite>` : Pour indiquer l'auteur de la citation
- Chaque testimonial doit être dans un article
- Les textes doivent être exactement comme montrés
- Garder le header existant

## Vérification :
- 3 blockquotes dans 3 articles
- Chaque citation a un auteur avec cite
- Textes exactement comme montrés
- Structure article > blockquote > p + cite

---

# TÂCHE 30 : Exemples de citations dans le styleguide

## Ce qu'il faut faire exactement :
1. Copier le fichier :
```bash
cp 28-styleguide.html 30-styleguide.html
```

2. Ajouter une nouvelle section :
```html
<section>
    <header>
        <h2>Blockquotes</h2>
    </header>
    <div>
        <h3>Inline quote</h3>
        <q>Stay hungry. Stay foolish.</q>
    </div>
    <div>
        <h3>Blockquote</h3>
        <blockquote>
            <p>I will be the leader of a company that ends up being worth billions of dollars, because I got the answers. I understand culture. I am the nucleus. I think that's a responsibility that I have, to push possibilities, to show people, this is the level that things could be at.</p>
            <cite>Kanye West, Musician</cite>
        </blockquote>
    </div>
</section>
```

## Explications très simples :
- Nouvelle section après Horizontal rule
- Montre 2 types de citations :
  1. `<q>` : citation courte en ligne
  2. `<blockquote>` : citation longue en bloc
- Les textes doivent être exactement comme montrés
- Noter la différence entre q et blockquote

## Vérification :
- Section placée au bon endroit
- Deux types de citations présents
- Textes copiés exactement
- Structure respectée avec header et divs

---

# TÂCHE 31 : Adresse et auteurs des news

## Ce qu'il faut faire exactement :
1. Copier le fichier :
```bash
cp 29-index.html 31-index.html
```

2. Ajouter l'adresse dans le footer :
```html
<footer>
    <address>
        234 Washington Street<br>
        Urbana, Illinois
    </address>
    <!-- Reste du footer -->
</footer>
```

3. Ajouter les auteurs aux articles de news :
```html
<article>
    <p>Career</p>
    <h3>Hoc loco tenere se Triarius non potuit.</h3>
    <p>Lorem ipsum dolor sit amet...</p>
    <small>By Kelly D.</small>
</article>
<!-- Répéter pour chaque article avec les auteurs :
- William A.
- Frances J. -->
```

## Explications très simples :
- `<address>` : Pour les adresses physiques
- `<br>` : Pour le saut de ligne dans l'adresse
- `<small>` : Pour les noms d'auteurs
- Ajouter l'auteur à la fin de chaque article
- Les textes doivent être exactement comme montrés

## Vérification :
- Adresse ajoutée au début du footer
- Saut de ligne dans l'adresse avec br
- Chaque article de news a son auteur
- Structure et textes exacts

# TÂCHE 32 : Section typographie

## Ce qu'il faut faire exactement :
1. Copier le fichier :
```bash
cp 30-styleguide.html 32-styleguide.html
```

2. Ajouter une nouvelle section Typography :
```html
<section>
    <header>
        <h2>Typography</h2>
    </header>
    <div>
        <address>
            320 Stewart Avenue, Unit 12<br>
            New York City NY 10001
        </address>
    </div>
    <div>
        <pre>
            <code>
                <h2>My title</h2>
                <p>Proin lacus turpis, feugiat sit amet sollicitudin non, volutpat in libero. Aenean hendrerit ultrices nulla ac lobortis. Vestibulum consectetur nibh vel ante rhoncus faucibus.</p>
            </code>
        </pre>
    </div>
    <div>
        <p>
            Curabitur sit amet turpis cursus massa mollis <mark>highlighted</mark>. Duis finibus leo massa, eget dapibus erat finibus sed. Aenean condimentum sapien magna, eleifend <mark>highlighted</mark> mi consequat ut. Cras nec quam sed sapien ultricies <mark>highlighted</mark> ut sed metus.
        </p>
    </div>
</section>
```

## Explications très simples :
- Cette section montre différents styles de texte :
  1. `<address>` : Pour une adresse formatée
  2. `<pre>` et `<code>` : Pour montrer du code
  3. `<mark>` : Pour surligner du texte
- Chaque exemple est dans son propre div
- Les textes doivent être exactement comme montrés

## Vérification :
- Section après la section Blockquotes
- Trois divs avec différents exemples
- Textes copiés exactement
- Balises utilisées correctement

---

# TÂCHE 33 : Table

## Ce qu'il faut faire exactement :
1. Copier le fichier :
```bash
cp 32-styleguide.html 33-styleguide.html
```

2. Ajouter une section avec une table :
```html
<section>
    <header>
        <h2>Table</h2>
    </header>
    <table>
        <caption>Star Wars Trilogy Data</caption>
        <thead>
            <tr>
                <th scope="col">Title</th>
                <th scope="col">Director</th>
                <th scope="col">Release Date</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <th scope="row">Star Wars: Episode IV - A New Hope</th>
                <td>George Lucas</td>
                <td>May 25th, 1977</td>
            </tr>
            <tr>
                <th scope="row">Star Wars: Episode V - The Empire Strikes Back</th>
                <td>Irvin Kershner</td>
                <td>May 21st, 1980</td>
            </tr>
            <tr>
                <th scope="row">Star Wars: Episode VI - Return of the Jedi</th>
                <td>Richard Marquand</td>
                <td>May 25th, 1983</td>
            </tr>
        </tbody>
    </table>
</section>
```

## Explications très simples :
- Nouvelle section après Typography
- Structure d'une table complète :
  * `<caption>` : Titre de la table
  * `<thead>` : En-tête avec les titres des colonnes
  * `<tbody>` : Corps avec les données
  * `<th scope="col">` : Pour les titres de colonnes
  * `<th scope="row">` : Pour les titres de lignes
  * `<td>` : Pour les données normales
- Les données doivent être exactement comme montrées

## Vérification :
- La structure de la table est complète
- Tous les scopes sont corrects
- Les dates sont au bon format
- Les textes sont exactement comme montrés

---

# TÂCHE 34 : Details

## Ce qu'il faut faire exactement :
1. Copier le fichier :
```bash
cp 33-styleguide.html 34-styleguide.html
```

2. Ajouter une section Details :
```html
<section>
    <header>
        <h2>Details</h2>
    </header>
    <div>
        <h3>Default</h3>
        <details>
            <summary>Show/Hide me</summary>
            <p>Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas.</p>
        </details>
    </div>
    <div>
        <h3>Open</h3>
        <details open>
            <summary>Always open</summary>
            <p>Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas.</p>
        </details>
    </div>
</section>
```

## Explications très simples :
- Nouvelle section après la table
- Deux exemples de `<details>` :
  1. Un fermé par défaut
  2. Un ouvert par défaut (attribut open)
- `<summary>` : Le texte qui apparaît toujours
- Le même paragraphe dans les deux details
- Les textes doivent être exactement comme montrés

## Vérification :
- Section placée au bon endroit
- Deux examples de details
- Premier sans attribut open
- Second avec attribut open
- Textes exactement comme montrés

# TÂCHE 35 : Remplacer le logo texte par une image

## Ce qu'il faut faire exactement :
1. Copier le fichier :
```bash
cp 31-index.html 35-index.html
```

2. Remplacer le span du logo dans le header :
```html
<header>
    <div>
        <div>
            <a href="/">
                <img src="logo-black.png" alt="Techium logo" width="160" height="40">
            </a>
        </div>
        <nav>
            <!-- Navigation existante -->
        </nav>
    </div>
</header>
```

3. Ajouter l'image dans le footer aussi :
```html
<footer>
    <img src="logo-black.png" alt="Techium logo" width="160" height="40">
    <!-- Reste du footer -->
</footer>
```

## Explications très simples :
- Remplacer le span "Techium" par une image
- L'image doit être :
  * Dans le lien du header
  * Au début du footer
- Attributs obligatoires :
  * src="logo-black.png"
  * alt="Techium logo"
  * width="160"
  * height="40"

## Vérification :
- Plus de span "Techium"
- Image dans le lien du header
- Image au début du footer
- Tous les attributs présents et corrects

---

# TÂCHE 36 : Ajouter des images dans les sections

## Ce qu'il faut faire exactement :
1. Copier le fichier :
```bash
cp 35-index.html 36-index.html
```

2. Ajouter des images dans 4 sections :

Works section (dans chaque article) :
```html
<article>
    <div>
        <img src="images/pic-work-01.jpg" alt="">
    </div>
    <h3><a href="#">Interior Design</a></h3>
</article>
<!-- Répéter pour les autres articles avec pic-work-02.jpg et pic-work-03.jpg -->
```

About Us section :
```html
<section>
    <div>
        <img src="images/pic-about-us.jpg" alt="" width="460" height="447">
        <h3>Who are we</h3>
        <!-- Reste du contenu -->
    </div>
</section>
```

Latest news section (dans chaque article) :
```html
<article>
    <div>
        <img src="images/pic-blog-01.jpg" alt="" width="305" height="205">
    </div>
    <!-- Reste du contenu de l'article -->
</article>
<!-- Répéter pour les autres articles avec pic-blog-02.jpg et pic-blog-03.jpg -->
```

Testimonials section (dans chaque article) :
```html
<article>
    <img src="images/pic-person-01.jpg" alt="Yuri Y. avatar" width="100" height="100">
    <blockquote>
        <!-- Citation existante -->
    </blockquote>
</article>
<!-- Répéter pour les autres articles avec pic-person-02.jpg et pic-person-03.jpg -->
```

## Explications très simples :
- Ajouter images dans 4 sections différentes
- Chaque image a ses propres attributs :
  * Works : pas de width/height
  * About : width="460" height="447"
  * News : width="305" height="205"
  * Testimonials : width="100" height="100"
- Les alt sont vides sauf pour les avatars
- Les noms des fichiers sont importants

## Vérification :
- Toutes les images ajoutées aux bons endroits
- Attributs corrects pour chaque image
- Alt vides sauf pour les avatars
- Structure div > img respectée quand nécessaire

---

# TÂCHE 37 : Icônes sociales

## Ce qu'il faut faire exactement :
1. Copier le fichier :
```bash
cp 36-index.html index.html
```

2. Remplacer les liens sociaux par des icônes SVG :
```html
<ul>
    <li>
        <a href="https://www.facebook.com/HolbertonSchool/">
            <svg viewbox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" width="25px" height="25px">
                <title>Facebook icon</title>
                <path d="M23.998 12c0-6.628-5.372-12-11.999-12C5.372 0 0 5.372 0 12c0 5.988 4.388 10.952 10.124 11.852v-8.384H7.078v-3.469h3.046V9.356c0-3.008 1.792-4.669 4.532-4.669 1.313 0 2.686.234 2.686.234v2.953H15.83c-1.49 0-1.955.925-1.955 1.874V12h3.328l-.532 3.469h-2.796v8.384c5.736-.9 10.124-5.864 10.124-11.853z"/>
            </svg>
        </a>
    </li>
    <!-- Répéter pour Twitter et Instagram avec leurs SVG respectifs -->
</ul>
```

## Explications très simples :
- Remplacer le texte des liens sociaux par des SVG
- Chaque SVG doit avoir :
  * viewbox correct
  * width="25px" height="25px"
  * title approprié
  * path avec le bon d=""
- Garder les liens et la structure ul/li

## Vérification :
- Plus de texte dans les liens sociaux
- SVG à la place avec tous les attributs
- Liens restent fonctionnels
- Structure ul > li > a > svg respectée

# TÂCHE 38 : Ajouter un lecteur vidéo dans le styleguide

## Ce qu'il faut faire exactement :
1. Copier le fichier :
```bash
cp 34-styleguide.html 38-styleguide.html
```

2. Ajouter une nouvelle section pour la vidéo :
```html
<section>
    <header>
        <h2>Video</h2>
    </header>
    <div>
        <video controls loop poster="https://intranet-projects-files.s3.amazonaws.com/webstack/thumbnail.jpg">
            <source src="https://intranet-projects-files.s3.amazonaws.com/webstack/BigBuckBunny.mp4" type="video/mp4">
            Sorry, your browser doesn't support HTML5 video
        </video>
    </div>
</section>
```

## Explications très simples :
- Nouvelle section après Details
- Balise `<video>` avec 3 attributs :
  * controls : affiche les boutons de contrôle
  * loop : la vidéo se répète
  * poster : image qui s'affiche avant lecture
- `<source>` : indique le fichier vidéo
- Texte de secours si la vidéo ne marche pas

## Vérification :
- Section placée au bon endroit
- Tous les attributs de video présents
- URL exactes pour poster et source
- Message de secours présent

---

# TÂCHE 39 : Ajouter un lecteur audio dans le styleguide

## Ce qu'il faut faire exactement :
1. Copier le fichier :
```bash
cp 38-styleguide.html 39-styleguide.html
```

2. Ajouter une section audio :
```html
<section>
    <header>
        <h2>Audio</h2>
    </header>
    <div>
        <audio controls>
            <source src="https://intranet-projects-files.s3.amazonaws.com/webstack/TroubleChapter8_64kb.mp3" type="audio/mpeg">
            Sorry, your browser doesn't support audio element
        </audio>
    </div>
</section>
```

## Explications très simples :
- Nouvelle section après la section Video
- Balise `<audio>` avec attribut controls
- Une seule source audio
- Message de secours si l'audio ne marche pas
- Structure identique à la section vidéo

## Vérification :
- Section après la section vidéo
- Audio avec controls
- URL exacte dans source
- Message de secours présent

---

# TÂCHE 40 : Iframe dans le styleguide (TÂCHE FINALE)

## Ce qu'il faut faire exactement :
1. Copier le fichier :
```bash
cp 39-styleguide.html styleguide.html
```

2. Ajouter la dernière section avec iframe :
```html
<section>
    <header>
        <h2>Iframe</h2>
    </header>
    <div>
        <iframe 
            width="350" 
            height="200" 
            src="https://www.youtube.com/embed/41N6bKO-NVI" 
            title="Holberton School">
            Holberton Sally
        </iframe>
    </div>
</section>
```

## Explications très simples :
- Dernière section du styleguide
- `<iframe>` avec attributs précis :
  * width="350"
  * height="200"
  * URL YouTube exacte
  * title spécifique
- Texte de secours à l'intérieur

## Vérification finale du styleguide complet :
1. Structure générale :
   - Toutes les sections dans l'ordre :
     * Headings
     * Paragraph
     * Lists
     * Horizontal rule
     * Blockquotes
     * Typography
     * Table
     * Details
     * Video
     * Audio
     * Iframe

2. Pour chaque section :
   - Header avec h2
   - Contenu correct
   - Indentation propre

3. Spécifiquement pour l'iframe :
   - Dimensions exactes
   - URL correcte
   - Titre présent
   - Texte de secours inclus

## Points importants finaux :
- Vérifier que tout le code est indenté correctement
- Tous les attributs sont écrits exactement comme montré
- Toutes les URLs sont correctes
- Tous les textes de secours sont présents
- La structure de chaque section est cohérente

Félicitations ! Vous avez terminé toutes les tâches du projet HTML avancé ! Chaque élément construit contribue à une base solide pour le développement web moderne.
