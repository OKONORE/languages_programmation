# 🔨 Modifications

## mkdocs.yml

### Infos site

???+code "Infos site"
    - Nom du site
    - URL du site
    - Description du Site
    - Copyright
        - Lien de redirection sur l'image de copyright
        - Image de copyright (ne fonctionne que sur la page Index)
        - Lien de redirection sur mon nom
    - Nav bar
        - Ajout de `- navigation.tracking` [documentation](https://squidfunk.github.io/mkdocs-material/setup/setting-up-navigation/#anchor-tracking)
    - Thème du site 
        - [custom_dir: overrides](modifications.fr.md#docsoverrides)
        - Couleurs
        - Logo sur l'onglet
        - logo sur le site
    - Social
        - github
            - lien
        - FranceIOI
            - lien
            - logo
        - Lichess
            - lien
            - [logo](https://fontawesome.com/icons/chess-pawn?s=solid)
    - Ajout du dépôt github
        - Changement du logo du dépôt sur le site (github logo)

### Extensions
???+code "Extensions"
    - Ajout de la barre de recherche
    - auto_title_map:
        - Ajout `"Lua" : "💻 Script LUA"`
        - Ajout `"Bash": "💻 Console lua"`
    - pymdownx.emoji:
        - 
    ```
    options:
        custom_icons:
        - overrides/.icons
    ```
        

### Support multi-langues
???+code "Support multi-langues"
    - Langues:
        - Support [Français](index.md)
        - Support [Anglais](index.en.md)
    - Ajout d'un selecteur de langues dans la barre du haut
        - Choix Français
        - Choix Anglais

### Extra
???+code "Extra"
    - styles CSS

## Plugins

???+code "Plugins"
    - Ajout du plugin video "[mkdocs_video](https://github.com/soulless-viewer/mkdocs-video)"
        - > Plugin permettant d'ajouter des vidéos
    - Ajout du plugin video "[mkdocs-git-revision-date-plugin](https://github.com/zhaoterryy/mkdocs-git-revision-date-plugin)"
        - > Plugin permettant d'ajouter la date de modification de la page en bas de la page
    - Ajout du plugin "[i18n](https://pypi.org/project/mkdocs-i18n/)" (pour le support multi-langues)
        - > permet de créer une "division" du site par langues, isolant les langues non sélectionées


### Options plugins

???+code "Options Plugins"
    - Modifications d'extension 
        - "auto_title_map"
            - Noms pour le LUA, Javascript
        - "pymdownx.tasklist"
        - custom_checkbox:    true
        - clickable_checkbox: false

## ci.yml

???+code "ci.yml"
    - passage du modèle [gitlab à un modèle github](https://squidfunk.github.io/mkdocs-material/publishing-your-site/#with-github-actions)
    - Modification pour permettre l'hébergement
        - voir [Mise en ligne](mise_en_ligne.fr.md)
    - script
        - ajout de ```- run: pip install mkdocs-video```
        - ajout de ```- run: pip install mkdocs-i18n```

## docs/scripts

???+code "docs/scripts"
    - Tout les scripts affichés sont stockés dans ```docs/scripts```
        - Scripts mermaid dans ```docs/scripts/mermaid```
        - Scripts python dans ```docs/scripts/python```
        - Scipts lua dans ```docs/scripts/lua```

## docs/css

???+code "docs/css"
    - Admonitions
        - ajout de l'admonition "code"
            - ???code
        - ajout de l'admonition "savoir"
            - ???savoir
        - Ajout de l'admonition "depot"
            - ???depot

## docs/overrides

???+code "docs/overrides"
    - ajouts de [commentaires](https://squidfunk.github.io/mkdocs-material/setup/adding-a-comment-system/)
        - overrides/main.html

### docs/overrides/.icons

???+code "docs/overrides/.icons"
    - Ajout de `chess-pawn-regular.svg`
        - :chess-pawn-regular:
    - Ajout `github-brands.svg`
        - :github-brands: