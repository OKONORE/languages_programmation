# Modifications

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
    - Thème du site 
        - Couleurs
        - Logo sur l'onglet
        - logo sur le site
    - Social
        - github
            - lien
        - FranceIOI
            - lien
            - logo
    - Ajout du dépôt github
        - Changement du logo du dépôt sur le site (github logo)

## Plugins

???+code "Plugins"
    - Ajout du plugin video "[mkdocs_video](https://github.com/soulless-viewer/mkdocs-video)"
        - > Plugin permettant d'ajouter des vidéos
    - Ajout du plugin video "[mkdocs-git-revision-date-plugin](https://github.com/zhaoterryy/mkdocs-git-revision-date-plugin)"
        - > Plugin permettant d'ajouter la date de modification de la page en bas de la page
    - Ajout de la barre de recherche

### Options Plugins

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
        - voir [Mise en ligne](mise_en_ligne.md)
    - script
        - ajout de ```python -m pip install mkdocs-video```

## docs/scripts

???+code "docs/scripts"
    - Tout les scripts affichés sont stockés dans ```docs/scripts```
        - Scripts mermaid dans ```docs/scripts/mermaid```
        - Scripts python dans ```docs/scripts/python```

## docs/css

???+code "docs/css"
    - Admonitions
        - ajout de l'admonition "code"
        - ajout de l'admonition "savoir"