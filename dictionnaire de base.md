Je vais commencer par le HTML, puis je continuerai avec le CSS. Je vais diviser cela en plusieurs parties claires avec des exemples de syntaxe.

# DICTIONNAIRE HTML DÉTAILLÉ

## 1. STRUCTURE DE BASE

```html
<!-- Structure minimale d'une page HTML -->
<!DOCTYPE html>              <!-- Déclare le type de document -->
<html lang="fr">            <!-- Début du document, définit la langue -->
    <head>                  <!-- En-tête avec métadonnées -->
        <meta charset="UTF-8">
        <title>Titre</title>
    </head>
    <body>                  <!-- Corps de la page -->
        <!-- Contenu -->
    </body>
</html>
```

## 2. BALISES STRUCTURELLES

```html
<!-- Exemple de structure sémantique -->
<header>
    <!-- En-tête de page: logo, navigation principale -->
    Utilisation: En haut de page
</header>

<nav>
    <!-- Navigation principale -->
    Utilisation: Menu, liens importants
    <ul>
        <li><a href="#">Lien</a></li>
    </ul>
</nav>

<main>
    <!-- Contenu principal -->
    Utilisation: Contenu unique à la page
</main>

<section>
    <!-- Section de contenu -->
    Utilisation: Grouper du contenu thématique
</section>

<article>
    <!-- Contenu autonome -->
    Utilisation: Blog post, article de news
</article>

<aside>
    <!-- Contenu secondaire -->
    Utilisation: Sidebar, infos complémentaires
</aside>

<footer>
    <!-- Pied de page -->
    Utilisation: Copyright, liens secondaires
</footer>
```

## 3. TEXTE ET FORMATAGE

```html
<!-- Titres - Hiérarchie de h1 à h6 -->
<h1>Titre principal</h1>     <!-- Un seul par page -->
<h2>Sous-titre</h2>         <!-- Sections principales -->
<h3>Sous-section</h3>       <!-- Sous-sections -->

<!-- Paragraphes et texte -->
<p>Paragraphe de texte</p>  <!-- Bloc de texte -->
<br>                        <!-- Saut de ligne -->
<hr>                        <!-- Ligne horizontale -->

<!-- Formatage texte -->
<strong>Important</strong>   <!-- Texte important -->
<em>Emphase</em>            <!-- Texte mis en valeur -->
<mark>Surligné</mark>       <!-- Texte surligné -->
<small>Petit texte</small>  <!-- Mentions légales, notes -->
```

## 4. LISTES

```html
<!-- Liste non ordonnée -->
<ul>
    <li>Élément</li>        <!-- Point -->
</ul>

<!-- Liste ordonnée -->
<ol>
    <li>Premier</li>        <!-- Numéroté -->
</ol>

<!-- Liste de définitions -->
<dl>
    <dt>Terme</dt>          <!-- Terme à définir -->
    <dd>Définition</dd>     <!-- Définition du terme -->
</dl>
```

## 5. MÉDIAS ET LIENS

```html
<!-- Images -->
<img src="image.jpg" 
     alt="Description"      <!-- Obligatoire pour accessibilité -->
     width="300" 
     height="200">

<!-- Liens -->
<a href="url">Texte</a>    <!-- Lien standard -->
<a href="#id">Ancre</a>    <!-- Lien interne -->
<a href="tel:+1234">Tel</a> <!-- Lien téléphone -->

<!-- Vidéo -->
<video controls>
    <source src="video.mp4" type="video/mp4">
</video>

<!-- Audio -->
<audio controls>
    <source src="audio.mp3" type="audio/mpeg">
</audio>
```

## 6. FORMULAIRES

```html
<!-- Structure formulaire -->
<form action="/submit" method="POST">
    <!-- Étiquette et champ -->
    <label for="nom">Nom:</label>
    <input type="text" id="nom" name="nom">

    <!-- Types d'input -->
    <input type="text">     <!-- Texte -->
    <input type="email">    <!-- Email -->
    <input type="password"> <!-- Mot de passe -->
    <input type="number">   <!-- Nombre -->
    <input type="checkbox"> <!-- Case à cocher -->
    <input type="radio">    <!-- Bouton radio -->
    
    <!-- Zone de texte -->
    <textarea></textarea>

    <!-- Liste déroulante -->
    <select>
        <option>Choix 1</option>
    </select>

    <!-- Bouton -->
    <button type="submit">Envoyer</button>
</form>
```
