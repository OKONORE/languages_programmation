# ⚙️ Mise en ligne

## Pourquoi mettre en ligne ?

!!!question "Pourquoi ?"
    Il peut être utile de mettre en ligne son site web pour pouvoir y accéder en ligne de partout dans le monde depuis son téléphone, et que tout le monde puisse y accéder.

## Comment le mettre en ligne

### Hébergement web

!!!Quote "Hébergement web"
    Héberger un site sur un serveur est la solution la plus pratiquée dans le monde, **mais** celà à un coût, il faut pouvoir louer une machine pour héberger un site, louer un nom de domaine et nécéssite des connaissances avancées dans la gestions de serveurs

### Github/Gitlab

!!!savoir 
    Voici le tutoriel de Mr.Chambon[^1]
    [^1]: [Le tutoriel](https://ens-fr.gitlab.io/mkdocs/gitlab-mkdocs/)

#### Fonctionnement Github

!!!info "Gitlab"
    Depuis un changement de politique de Gitlab, une carte bancaire doit être entrée pour pouvoir bénificier de l'hébergement de Gitlab.


Tout d'abord, il vous faut un fichiers mkdocs valide, que vous enverrez sur le dépot github depuis votre interface de développement. Ensuite Github lancera les fonctions dans le fichier d'intégration continue, et si tout se passe bien, le site sera publié.






```mermaid
--8<-- "docs/scripts/mermaid/github_deploy"
```
```mermaid
--8<-- "docs/scripts/mermaid/branches_github"
```

