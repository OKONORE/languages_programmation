# Modifications

## mkdocs.yml

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
    - Logo onglet
    - logo sur le site
- Ajout du plugin video "[mkdocs_video](https://github.com/soulless-viewer/mkdocs-video)"
- Ajout de la barre de recherche
- Modifications d'extension 
    - "auto_title_map"
        - Noms pour le LUA, Javascript
    - "pymdownx.tasklist"
       - custom_checkbox:    true
       - clickable_checkbox: false
- Social
    - github
        - lien
    - FranceIOI
        - lien
        - logo

## ci.yml

- Modification pour permettre l'hébergement
    - voir [Mise en ligne](mise_en_ligne.md)
- script
    - ajout de "python -m pip install mkdocs-video"


## /scripts

- Tout les scripts affichés sont stockés dans ```docs/scripts```