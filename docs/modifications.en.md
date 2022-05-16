# 🔨 Changes

## mkdocs.yml

### Site info

???+code "Site info"
    - Name of the site
    - Site URL
    - Site description
    - Copyright
        - Redirect link to copyright image
        - Copyright image (only works on the Index page)
        - Redirect link to my name
    - Nav bar
        - Added `navigation.tracking` [documentation](https://squidfunk.github.io/mkdocs-material/setup/setting-up-navigation/#anchor-tracking)
    - Theme of the site 
        - custom_dir: [overrides](modifications.en.md#docsoverrides)
        - Colors
        - Logo on the tab
        - logo on the site
    - Social
        - github
            - link
        - FranceIOI
            - link
            - logo
        - Lichess
            - link
            - [logo](https://fontawesome.com/icons/chess-pawn?s=solid)
    - Adding the github repository
        - Changed the logo of the repository on the site (github logo)

### Extensions
???+code "Extensions"
    - Adding the search bar
    - auto_title_map:
        - Added `"Lua": "💻 LUA script"`
        - Added `"Bash": "💻 Console lua"`
    - pymdownx.emoji:
        - 
    ```
    options:
        custom_icons:
        - overrides/.icons
    ```
        

### Multi-language support
???+code "Multi-language support"
    - Languages:
        - Support [French](index.md)
        - Support [English](index.en.md)
    - Add a language selector in the top bar
        - French choice
        - English choice

### Extra
???+code "Extra"
    - CSS styles

## Plugins

???+code "Plugins"
    - Added video plugin "[mkdocs_video](https://github.com/soulless-viewer/mkdocs-video)"
        - > Plugin to add videos
    - Added video plugin "[mkdocs-git-revision-date-plugin](https://github.com/zhaoterryy/mkdocs-git-revision-date-plugin)"
        - > Plugin to add the date of modification of the page at the bottom of the page
    - Added plugin "[i18n](https://pypi.org/project/mkdocs-i18n/)" (for multi-language support)
        - > Allows to create a "division" of the site by languages, isolating the unselected languages


### Plugins options

???+code "Plugin options"
    - Extension changes 
        - "auto_title_map"
            - Names for LUA, Javascript
        - "pymdownx.tasklist"
        - custom_checkbox: true
        - clickable_checkbox: false

## ci.yml

???+code "ci.yml"
    - change from [gitlab to github](https://squidfunk.github.io/mkdocs-material/publishing-your-site/#with-github-actions)
    - Modification to allow hosting
        - see [Putting online](mise_en_ligne.fr.md)
    - script
        - added `- run: pip install mkdocs-video`
        - added `- run: pip install mkdocs-i18n`

## docs/scripts

???+code "docs/scripts"
    - All displayed scripts are stored in `docs/scripts`
        - mermaid scripts in `docs/scripts/mermaid`
        - Python scripts in `docs/scripts/python`
        - Lua scripts in `docs/scripts/lua`

## docs/css

???+code "docs/css"
    - Admonitions
        - added admonition "code
            - ???code
        - added admonition "knowledge
            - ???savoir
        - added admonition "depot
            - ???depot

## docs/overrides

???+code "docs/overrides"
    - additions of [comments](https://squidfunk.github.io/mkdocs-material/setup/adding-a-comment-system/)
        - overlays/main.html

### docs/overrides/.icons

???+code "docs/overrides/.icons"
    - added `chess-pawn-regular.svg`
        - :chess-pawn-regular:
    - added `github-brands.svg`
        - :github-brands: