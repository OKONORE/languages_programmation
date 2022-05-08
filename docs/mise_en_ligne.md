# ⚙️ Mise en ligne

## Pourquoi mettre en ligne ?

!!!question "Pourquoi ?"
    Il peut être utile de mettre en ligne son site web[^1] pour pouvoir y accéder en ligne de partout dans le monde depuis son téléphone, et que tout le monde puisse y accéder.
    [^1]: [Wikipedia: Web Hosting Service](https://en.wikipedia.org/wiki/Web_hosting_service)
## Comment le mettre en ligne

### Hébergement web

!!!Quote "Hébergement web"
    Héberger un site sur un serveur est la solution la plus pratiquée dans le monde, **mais** celà à un coût, il faut pouvoir louer une machine pour héberger un site, louer un nom de domaine et nécéssite des connaissances avancées dans la gestions de serveurs
    
    ???+example "Exemples"
        === "OVH"

            ![ovh logo](images/ovh.png)
            > [OVH](https://www.ovhcloud.com/fr/) est est une entreprise française. Elle pratique initialement de l'hébergement de serveur, et est un fournisseur d'accès à Internet (FAI), puis opérateur de télécommunications pour les entreprises. Elle se développe, à la fin des années 2010, dans le cloud computing (informatique en nuage).
            **Source: Wikipedia[^3]**
            [^3]: [Wikipedia: OVHcloud](https://fr.wikipedia.org/wiki/OVHcloud)

            **[Comparatif de prix](https://www.ovhcloud.com/fr/web-hosting/):**

            |HÉBERGEMENT PERSO|HÉBERGEMENT PRO|HÉBERGEMENT PERFORMANCE|HÉBERGEMENT CLOUD WEB|
            |:---:|:---:|:---:|:---:|
            | ![offre 1](images/offresOVH/1.PNG) | ![offre 2](images/offresOVH/2.PNG) | ![offre 3](images/offresOVH/3.PNG) | ![offre 4](images/offresOVH/4.PNG) |

        === "Bluehost"

            ![bluehost logo](images/bluehost.png)
            > [Bluehost](https://www.bluehost.com/) est une société d'hébergement Web appartenant à Endurance International Group. C'est l'un des 20 plus grands hébergeurs Web, hébergeant collectivement plus de 2 millions de domaines.
            **Source: Wikipedia[^4]**
            [^4]: [Wikipedia: Bluehost](https://en.wikipedia.org/wiki/Bluehost)

            **[Comparatif de prix](https://www.bluehost.com/hosting/shared):**

            |BASIC|PLUS|CHOICE PLUS|PRO|
            |:---:|:---:|:---:|:---:|
            | ![offre 1](images/offresBluehost/1.PNG) | ![offre 2](images/offresBluehost/2.PNG) | ![offre 3](images/offresBluehost/3.PNG) | ![offre 4](images/offresBluehost/4.PNG) |

        === "Vous même"

        !!!tip "Info"
            Effectivement, vous pouvez vous même héberger un site web chez vous. Il vous suffit pour ça d'avoir une vielle machine/ordinateur, disponible en permanence, et de paramétrer  votre connection pour accepter les requêtes exterieures.
        !!!savoir "tutoriel"
            Voici un tutoriel pour faire cela: [Tutoriel](https://web.developpez.com/cours/serveur-web-chez-soi/#:~:text=Solution%20simple%20%3A%20vous%20passez%20par,IP%20de%20votre%20connexion%20Internet.)

### Github/Gitlab

!!!savoir "Tutoriel"
    Voici le tutoriel de Mr.Chambon[^2]
    [^2]: [Le tutoriel](https://ens-fr.gitlab.io/mkdocs/gitlab-mkdocs/)

!!!caution "Gitlab"
    Depuis un changement de politique de Gitlab, une carte bancaire doit être entrée pour pouvoir bénificier de l'hébergement de Gitlab. Il ne sera donc pas présenté ici.

#### Fonctionnement Github

!!!help "comment ?"
    1. il vous faut un fichier contenant toutes vos pages, images, et autre au format mkdocs
    2. Vous enverrez ces fichiers sur le dépot github depuis votre interface de développement
    2. Github lancera l'intégration continue avec les paramètres dans `ci.yml`
    3. Github héberge votre page web issue de vos fichiers Mkdocs

    ```mermaid
    --8<-- "docs/scripts/mermaid/github_deploy"
    ```

### Branches Github

!!!example "détails"
    > Github a de base une branche "**main**", qui a pour rôle de branche principale

    1. Github lance l'intégration continue
    2. la commande `- run: mkdocs gh-deploy --force` transforme le markdown en HTML
    3. La page HTML est stockée dans la branche "**gh-pages**"
    4. L'environnement [Github Pages](https://pages.github.com/) lance le site depuis `gh-pages/root`
    5. Le site est disponible à: `<pseudonyme>.github.io/<nom_dépôt>`

    ```mermaid
    --8<-- "docs/scripts/mermaid/branches_github"
    ```

*[HTML]: Hyper Text Markup Language