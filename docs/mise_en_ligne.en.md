# ⚙️ Putting it online

## Why put online?

!!!question "Why ?"
    It can be useful to put your website online[^wiki1] so that you can access it online from anywhere in the world from your phone, and everyone can access it.
    [^wiki1]: [Wikipedia: Web Hosting Service](https://en.wikipedia.org/wiki/Web_hosting_service)
## How to put it online

### Web hosting

!!!Quote "Web hosting"
    Hosting a site on a server is the most common solution in the world, but** it has a cost, you need to rent a machine to host a site, rent a domain name and requires advanced knowledge in server management
    
    ???+example "Examples"
        === "OVH"

            ![ovh logo](images/ovh.png){ width=200 }
            > [OVH](https://www.ovhcloud.com/fr/) is a French company. It initially practices server hosting, and is an Internet Service Provider (ISP), then a telecommunications operator for businesses. It develops, in the late 2010s, in the cloud computing.
            **Source: Wikipedia[^3]**
            [^3]: [Wikipedia: OVHcloud](https://fr.wikipedia.org/wiki/OVHcloud)

            **[Price comparison](https://www.ovhcloud.com/fr/web-hosting/):**

            |HÉBERGEMENT PERSO|HÉBERGEMENT PRO|HÉBERGEMENT PERFORMANCE|HÉBERGEMENT CLOUD WEB|
            |:---:|:---:|:---:|:---:|
            | ![offre 1](images/offresOVH/1.PNG){ width=150 } | ![offre 2](images/offresOVH/2.PNG){ width=150 } | ![offre 3](images/offresOVH/3.PNG){ width=150 }| ![offre 4](images/offresOVH/4.PNG){ width=150 } |

        === "Bluehost"

            ![bluehost logo](images/bluehost.png){ width=200 }
            > [Bluehost](https://www.bluehost.com/) is a web hosting company owned by Endurance International Group. It is one of the top 20 web hosting companies, collectively hosting over 2 million domains.
            **Source: Wikipedia[^4]**
            [^4]: [Wikipedia: Bluehost](https://en.wikipedia.org/wiki/Bluehost)

            **[Price comparison](https://www.bluehost.com/hosting/shared):**

            |BASIC|PLUS|CHOICE PLUS|PRO|
            |:---:|:---:|:---:|:---:|
            | ![offre 1](images/offresBluehost/1.PNG){ width=150 } | ![offre 2](images/offresBluehost/2.PNG){ width=150 } | ![offre 3](images/offresBluehost/3.PNG){ width=150 } | ![offre 4](images/offresBluehost/4.PNG){ width=150 } |

        === "Yourself"

            !!!tip "Info"
                Indeed, you can host a web site at home. You just need to have an old machine/computer, permanently available, and to set up your connection to accept external requests.
            !!!savoir "tutorial"
                Here is a tutorial to do this: [Tutorial](https://web.developpez.com/cours/serveur-web-chez-soi/#:~:text=Solution%20simple%20%3A%20you%20go%20through,IP%20of%20your%20Internet%20connection.)

### Github/Gitlab

!!!savoir "Tutorial"
    Here is the tutorial of Mr.Chambon[^tuto1]
    [^tuto1]: [The tutorial](https://ens-fr.gitlab.io/mkdocs/gitlab-mkdocs/)

!!!caution "Gitlab"
    Since a change in Gitlab's policy, a credit card must be entered to benefit from Gitlab's hosting. It will therefore not be presented here.

#### Github Functioning

!!!help "how?"
    1. you need a file containing all your pages, images, and such in mkdocs format
    2. You will upload these files to the github repository from your development interface
    2. Github will launch the continuous integration with the parameters in `ci.yml`
    3. Github hosts your web page from your Mkdocs files

    ```mermaid
    --8<-- "docs/scripts/mermaid/github_deploy.en"
    ```

!!!example "details"
    > Github has a basic branch "_main_", which has the role of main branch

    1. Github starts the continuous integration
    2. the command `- run: mkdocs gh-deploy --force` transforms the markdown into HTML
    3. The HTML page is stored in the "**gh-pages**" branch
    4. The [Github Pages] environment (https://pages.github.com/) launches the site from `gh-pages/root`
    5. The site is available at: `<pseudonym>.github.io/<deposit_name>`

    ```mermaid
    --8<-- "docs/scripts/mermaid/branches_github.en"
    ```

*[HTML]: Hyper Text Markup Language