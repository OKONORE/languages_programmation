# 💻 Le lua

!!!note "Définition"
    Lua est un [langage de script](https://fr.wikipedia.org/wiki/Langage_de_script) [libre](https://fr.wikipedia.org/wiki/Logiciel_libre), [réflexif](https://fr.wikipedia.org/wiki/R%C3%A9flexion_(informatique)) et [impératif](https://fr.wikipedia.org/wiki/Programmation_imp%C3%A9rative).

---

???tldr "Définition Longue"
    Créé en [1993](https://fr.wikipedia.org/wiki/1993_en_informatique), il est conçu de manière à pouvoir être embarqué au sein d'autres applications afin d'étendre celles-ci. Lua (du portugais : Lua [ˈlu.ɐ], au Brésil : [ˈlu.a], signifiant « Lune ») a été développé par Luiz Henrique de Figueiredo, Roberto Ierusalimschy (en) et Waldemar Celes, membres du groupe de recherche TeCGraf, de l'[université pontificale catholique de Rio de Janeiro](https://fr.wikipedia.org/wiki/Universit%C3%A9_pontificale_catholique_de_Rio_de_Janeiro) au [Brésil](https://fr.wikipedia.org/wiki/Br%C3%A9sil).

    L'interpréteur Lua est écrit en [langage C](https://fr.wikipedia.org/wiki/C_(langage)) [ANSI](https://fr.wikipedia.org/wiki/ANSI) strict, et de ce fait est compilable sur une grande variété de systèmes. Il est également très compact, la version 5.0.2 n'occupant que 95 ko à 185 ko selon le compilateur utilisé et le système cible. Il est souvent utilisé dans des [systèmes embarqués](https://fr.wikipedia.org/wiki/Syst%C3%A8me_embarqu%C3%A9) tels qu'[OpenWrt](https://fr.wikipedia.org/wiki/OpenWrt) où cette compacité est très appréciée. Il profite de la compatibilité que possède le langage C avec un grand nombre de langages pour s'intégrer facilement dans la plupart des projets. Il intègre un [ramasse-miettes](https://fr.wikipedia.org/wiki/Ramasse-miettes_(informatique)).

    Il est particulièrement apprécié pour l'embarqué, le développement [réseau](https://fr.wikipedia.org/wiki/R%C3%A9seau) et les [jeux vidéo](https://fr.wikipedia.org/wiki/Jeu_vid%C3%A9o).

    Le Lua est utilisé dans des jeux vidéo comme : Transformice, World of Warcraft, Roblox, Garry's Mod, Onset, computercraft mod (mod de Minecraft), Multi Theft Auto (mod multijoueur de Grand Theft Auto: San Andreas), FiveM (mod multijoueur de Grand Theft Auto V), Factorio, ainsi que les moteurs de jeu vidéo tels que le SourceEngine, CryENGINE, LÖVE, ou encore les Fantasy consoles, tel que Pico-8.

    Il est également utilisé au niveau réseau comme hook sur Apache, Lighttpd (par défaut), Nginx (via OpenResty), dans les routeurs Cisco, dans l'analyseur de paquets Wireshark, l'antispam Rspamd, l'autocommutateur téléphonique privé Asterisk (optionnel), pour les scripts de MediaWiki.
    
__*source: Wikipedia[^wiki1]*__
[^wiki1]: [Wikipedia : Lua](https://fr.wikipedia.org/wiki/Lua)

- [X] Orienté Procédural[^orien1]
- [X] Orienté Fonctionel[^orien2]
- [ ] Orienté Objet[^orien3]

[^orien1]: [Wikipedia : Programmation procédurale](https://fr.wikipedia.org/wiki/Programmation_proc%C3%A9durale)
[^orien2]: [Wikipedia : Programmation fonctionnelle](https://fr.wikipedia.org/wiki/Programmation_fonctionnelle)
[^orien3]: [Wikipedia : Programmation orientée objet](https://fr.wikipedia.org/wiki/Programmation_orient%C3%A9e_objet)

## Exemples de codes

### HelloWorld

- Pour commencer, nous allons voir comment écrire `helloworld` dans la console lua:

!!!Note "Ecrire `helloworld`"

    === "Code 1"
        !!!Success "Réussite"
            === "lua"
                En lua:
                ```lua linenums="1"
                --8<-- "docs/scripts/lua/helloworld/helloworld1.lua"
                ```
                ```bash
                --8<-- "docs/scripts/lua/helloworld/helloworld1console.lua"
                ```

            === "python"   
                Comparaison Python:    
                ```python linenums="1"
                --8<-- "docs/scripts/python/helloworld/helloworld1.py"
                ```
                ```pycon
                --8<-- "docs/scripts/python/helloworld/helloworld1console.py"
                ```
            
    === "Code 2"
        !!!failure "Erreur"
            === "lua" 
                En lua:
                ```lua linenums="1"
                --8<-- "docs/scripts/lua/helloworld/helloworld2.lua"
                ```
                ```bash
                --8<-- "docs/scripts/lua/helloworld/helloworld2console.lua"
                ```

            === "python" 
                Comparaison Python:
                ```python linenums="1" hl_lines="1"
                --8<-- "docs/scripts/python/helloworld/helloworld2.py"
                ```
                ```pycon
                --8<-- "docs/scripts/python/helloworld/helloworld2console.py"
                ```

### Boucles

- Ici, nous allons voir comment faire une boucle qui envoi dans la console les chiffres de 0 à 10 inclus.

!!!Note "Ecrire `helloworld`"

    === "Code 1"
        !!!Success "Réussite"
            === "lua"
                En lua:
                ```lua linenums="1"
                --8<-- "docs/scripts/lua/boucles/boucle1.lua"
                ```
                ```bash
                --8<-- "docs/scripts/lua/boucles/boucle1console.lua"
                ```

            === "python"   
                Comparaison Python:    
                ```python linenums="1"
                --8<-- "docs/scripts/python/boucles/boucle1.py"
                ```
                ```pycon
                --8<-- "docs/scripts/python/boucles/boucle1console.py"
                ```
            
    === "Code 2"
        !!!failure "Erreur"
            === "lua"
                En lua:
                ```lua linenums="1"
                --8<-- "docs/scripts/lua/boucles/boucle2.lua"
                ```
                ```bash
                --8<-- "docs/scripts/lua/boucles/boucle2console.lua"
                ```

            === "python"   
                Comparaison Python (qui fonctionne):    
                ```python linenums="1"
                --8<-- "docs/scripts/python/boucles/boucle2.py"
                ```
                ```pycon
                --8<-- "docs/scripts/python/boucles/boucle2console.py"
                ```

### Mathématiques

!!!note "Mathématiques"
    Lua, est tout comme python, un outil permettant de faire des mathématiques.

- Ici nous allons voir comment transformer cette formule en un code lua, qui nous renverras le résulat dans la console

$$
\Delta = b^2-4ac
$$

> Cette formule permet de calculer Delta

!!!Note "Mathématiques"

    === "Code 1"
        !!!Success "Réussite"
            === "lua"
                En lua:
                ```lua linenums="1"
                --8<-- "docs/scripts/lua/delta/delta1.lua"
                ```
                ```bash
                --8<-- "docs/scripts/lua/delta/delta1console.lua"
                ```

            === "python"   
                Comparaison Python:    
                ```python linenums="1"
                --8<-- "docs/scripts/python/delta/delta1.py"
                ```
                ```pycon
                --8<-- "docs/scripts/python/delta/delta1console.py"
                ```
    
    === "Code 2"
        !!!Success "Réussite"
            === "lua"
                En lua:
                ```lua linenums="1"
                --8<-- "docs/scripts/lua/delta/delta2.lua"
                ```
                ```bash
                --8<-- "docs/scripts/lua/delta/delta2console.lua"
                ```
            === "python"   
                Comparaison Python:    
                ```python linenums="1"
                --8<-- "docs/scripts/python/delta/delta2.py"
                ```
                ```pycon
                --8<-- "docs/scripts/python/delta/delta2console.py"
                ```

    === "Code 3"
        !!!failure "Erreur"
            === "lua"
                En lua:
                ```lua linenums="1"
                --8<-- "docs/scripts/lua/delta/delta3.lua"
                ```
                ```bash
                --8<-- "docs/scripts/lua/delta/delta3console.lua"
                ```
            === "python"   
                Comparaison Python:    
                ```python linenums="1" hl_lines="2"
                --8<-- "docs/scripts/python/delta/delta3.py"
                ```
                ```pycon
                --8<-- "docs/scripts/python/delta/delta3console.py"
                ```

### Listes

- Ici nous allons voir un exemple pour envoyer chaque élements d'une liste dans la console

!!!Note "Listes"

    === "Code 1"
        !!!Success "Réussite"
            === "lua"
                En lua:
                ```lua linenums="1"
                --8<-- "docs/scripts/lua/listes/listes1.lua"
                ```
                ```bash
                --8<-- "docs/scripts/lua/listes/listes1console.lua"
                ```
            === "python"
                Comparaison Python:
                ```python linenums="1"
                --8<-- "docs/scripts/python/listes/listes1.py"
                ```
                ```pycon
                --8<-- "docs/scripts/python/listes/listes1console.py"
                ```
    
    === "Code 2"
        !!!Success "Réussite"
            === "lua"
                En lua:
                ```lua linenums="1"
                --8<-- "docs/scripts/lua/listes/listes2.lua"
                ```
                ```bash
                --8<-- "docs/scripts/lua/listes/listes2console.lua"
                ```
            === "python"
                Comparaison Python:
                ```python linenums="1"
                --8<-- "docs/scripts/python/listes/listes2.py"
                ```
                ```pycon
                --8<-- "docs/scripts/python/listes/listes2console.py"
                ```

## Projets personnels en lua

!!!info "Projets"
    J'ai personnellement des projets qui sont créés en lua.

### Hestia RolePlay

!!!quote "Hestia RolePlay"

    ![HestiaRP logo](images/logo_hestia.webp){ align=right }
    Depuis plusieurs années, je m'intéresse à la programmation de serveurs multijoueurs en lua sur Garry's Mod[^gmod].
    [^gmod]: [Facepunch](https://gmod.facepunch.com/) & [Wikipedia: Garry's Mod](https://en.wikipedia.org/wiki/Garry%27s_Mod)

    Depuis peu, des amis et moi avons commencé l'élaboration d'un serveur multijoueur ensemble.
    Je m'occupe personellement de la programmation de tout le serveur.

    Mes amis eux, s'occupent du site web, de l'hébergement du serveur, de la communautée, du design et de la charte graphique.

    Notre projet en est vraiement à ses débuts.

    Voici notre [site web](https://www.hestia-rp.fr/)

!!!info "Serveurs Gmod"

    [https://wiki.facepunch.com/gmod](https://wiki.facepunch.com/gmod)

### Crosshair HUD

!!!quote "Crosshair HUD"
    J'ai, pour mon serveur, développé plusieurs scripts. Celui ci est un script assez simple permettant d'avoir un pointeur personalisable sur notre écran dans le jeu Garry's Mod[^gmod].
    
    | Menu de configuration | Rendu du pointeur |
    |:---:|:---:|
    | ![image menu](images/menu_crosshair.PNG){ width=415 } | ![image menu](images/rendu_crosshair.PNG){ width=500 } |

!!!depot "Dépôt"
    :github-brands: Voici le dépot de ce mod: [crosshair_gmod](https://github.com/OKONORE/crosshair_gmod)
    { align=center }

### Mod de modération

!!!quote "Système de Modération"
    J'ai aussi un début de mod permettant de faire de la modération sur le serveur, mais aucuns aperçu ne pourra être donné maintenant, car le mod n'est pas assez avancé mettant en jeu des bases de données SQL, des API et des bots (peut-être dans une future mise à jour du site)
    
### Interface de personnage

!!!quote "CleanHUD"

    !!!info "Informations"
        ![CleanHUD logo](images/rendu_HUD/logo_cleanhud.png){ align=right width=500}
        Le HUD que j'ai développé, est une interface permettant d'avoir des informations principales de son personnages affichés sur son écran.
    
    ???+danger "images"
        En voici des images (les images sont en anglais car le public visé était anglais ; images réalisés par un amis):

        | Image 1 |
        |:---:|
        |![CleanHUD image 1](images/rendu_HUD/1.png)|
        | **Image 2** |
        |![CleanHUD image 2](images/rendu_HUD/2.png)|
        | **Image 3** |
        |![CleanHUD image 3](images/rendu_HUD/3.png)|
        | **Image 4** |
        |![CleanHUD image 4](images/rendu_HUD/4.png)|

        
    
    !!!depot "Dépôt" 
        :github-brands: Voici le dépot de ce mod: [CleanHUD](https://github.com/OKONORE/CleanHUD)
        { align=center }
        
        P.S: Ajouté pour l'occasion
        { align=center }

### Mod Factorio

!!!quote "FactoWorldWars"
    Ce mod est cette fois un mod de Factorio[^factorio].
    Ce mod a pour objectif de transformer Factorio en jeu de stratégie et logistique.
    Il est **^^très loin^^** d'être fini, et est pour l'instant mit de côté. Il est développé par moi et un autre ami.
    [^factorio]: [Factorio](https://www.factorio.com/) & [Wikipedia: Factorio](https://en.wikipedia.org/wiki/Factorio)

    [FactoWorld Wars](https://mods.factorio.com/mod/Factoworldwars)

*[HUD]: Head-up display
