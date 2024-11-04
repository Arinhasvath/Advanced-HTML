# Advanced-HTML

# Guide d'installation de l'environnement de développement Web

## 1. Éditeur de code

### VS Code (Recommandé)
1. Télécharger : [Visual Studio Code](https://code.visualstudio.com/)
2. Extensions essentielles à installer :
   - Live Server
   - HTML CSS Support
   - Auto Close Tag
   - Auto Rename Tag
   - Prettier - Code formatter
   - ESLint
   - PHP Intelephense
   - GitLens

### Alternative : Sublime Text
- Télécharger : [Sublime Text](https://www.sublimetext.com/)
- Plus léger que VS Code mais moins de fonctionnalités

## 2. Navigateurs

### Navigateurs principaux
1. Google Chrome (Principal)
   - Télécharger : [Chrome](https://www.google.com/chrome/)
   - Extensions :
     * DevTools
     * Web Developer
     * ColorZilla
     * Dimensions

2. Firefox Developer Edition (Pour tests)
   - Télécharger : [Firefox Developer](https://www.mozilla.org/fr/firefox/developer/)

## 3. Configuration PHP

### Windows
1. Télécharger XAMPP :
   - Aller sur [XAMPP](https://www.apachefriends.org/)
   - Télécharger la version avec PHP 8+
   - Installation :
     ```
     - Choisir les composants : Apache, MySQL, PHP, phpMyAdmin
     - Installer dans C:\xampp
     - Lancer XAMPP Control Panel
     - Activer Apache et MySQL
     ```

### Mac
1. Installer MAMP :
   - Télécharger [MAMP](https://www.mamp.info/)
   - Installation simple : suivre l'assistant
   - Lancer MAMP
   - Configurer les ports si nécessaire

### Linux (Ubuntu/Debian)
```bash
# Mettre à jour le système
sudo apt update
sudo apt upgrade

# Installer Apache
sudo apt install apache2

# Installer PHP
sudo apt install php libapache2-mod-php php-mysql

# Installer MySQL
sudo apt install mysql-server

# Installer phpMyAdmin
sudo apt install phpmyadmin
```

## 4. Outils de gestion de version

### Git
1. Windows : 
   - Télécharger [Git for Windows](https://gitforwindows.org/)
   - Installer avec options par défaut

2. Mac :
   - Installer via Terminal :
   ```bash
   brew install git
   ```

3. Linux :
   ```bash
   sudo apt install git
   ```

## 5. Configuration du projet

### Structure des dossiers
```
mon_projet/
├── html_advanced/
│   ├── images/
│   ├── styles/
│   └── index.html
├── css_advanced/
└── php/
```

### Commandes pour créer la structure
```bash
# Créer les dossiers
mkdir -p mon_projet/{html_advanced/{images,styles},css_advanced,php}

# Se placer dans le dossier du projet
cd mon_projet

# Initialiser git
git init
```

## 6. Extensions VS Code recommandées supplémentaires

### Pour HTML/CSS
- HTML Snippets
- CSS Peek
- HTML CSS Class Completion
- IntelliSense for CSS
- Live Sass Compiler (si vous utilisez SASS)

### Pour PHP
- PHP Debug
- PHP Extension Pack
- PHP Namespace Resolver

## 7. Configuration VS Code

1. Ouvrir Settings (Ctrl/Cmd + ,)
2. Ajouter ces configurations :
```json
{
    "editor.formatOnSave": true,
    "editor.defaultFormatter": "esbenp.prettier-vscode",
    "editor.tabSize": 2,
    "editor.wordWrap": "on",
    "files.autoSave": "afterDelay",
    "files.autoSaveDelay": 1000
}
```

## 8. Outils supplémentaires utiles

### Design
- Figma (gratuit) : [https://www.figma.com/](https://www.figma.com/)
- Adobe Color : [https://color.adobe.com/](https://color.adobe.com/)

### Performance
- PageSpeed Insights : [https://pagespeed.web.dev/](https://pagespeed.web.dev/)
- GTmetrix : [https://gtmetrix.com/](https://gtmetrix.com/)

### Validation
- W3C Markup Validator : [https://validator.w3.org/](https://validator.w3.org/)
- W3C CSS Validator : [https://jigsaw.w3.org/css-validator/](https://jigsaw.w3.org/css-validator/)

## 9. Workflow recommandé

1. Développement HTML :
   - Travailler dans `/html_advanced`
   - Utiliser Live Server pour voir les changements en direct
   - Valider régulièrement avec W3C

2. Développement CSS (prochaine étape) :
   - Travailler dans `/css_advanced`
   - Utiliser l'inspecteur Chrome/Firefox
   - Tester sur différents navigateurs

3. PHP (plus tard) :
   - Travailler dans `/php`
   - Utiliser XAMPP/MAMP pour le serveur local
   - Tester avec différentes versions de PHP

## 10. Commandes utiles

```bash
# Lancer le serveur PHP local
php -S localhost:8000

# Vérifier les versions installées
php -v
git --version
node -v

# Créer un fichier HTML de base
touch index.html

# Ouvrir VS Code dans le dossier actuel
code .
```

## Points importants :
1. Toujours travailler avec un serveur local (Live Server ou PHP)
2. Sauvegarder régulièrement
3. Valider le code régulièrement
4. Tester sur différents navigateurs
5. Utiliser le contrôle de version (git)
