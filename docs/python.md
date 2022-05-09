# Le langage 🐍 Python

## Définition

!!!tldr "Définition"
    Le Python est un langage de programmation interprété, multi-paradigme et multiplateformes. Il favorise la programmation impérative structurée, fonctionnelle et orientée objet. Il est doté d'un typage dynamique fort, d'une gestion automatique de la mémoire par ramasse-miettes et d'un système de gestion d'exceptions.
    __*source: Wikipedia[^1]*__
    [^1]: [Wikipedia : Definition](https://fr.wikipedia.org/wiki/Python_(langage))

- [X] Orienté Fonctionelle    
- [X] Orientée Objet

!!!tldr "Info"
    Nous présentons rapidement le pyton afin d'avoir un comparatif avec les langages qui seront présentés après
## Exemples de codes

### HelloWorld

- Pour commencer, nous allons voir comment écrire `helloworld` dans la console python:

!!!Note "Ecrire `helloworld`"

    === !!!Success "Réussite"
            ```python linenums="1"
            --8<-- "docs/scripts/python/helloworld/helloworld1"
            ```
            Voici ici comment écrire `helloworld` dans la console. La fonction `print` sert à écrire dans la console ce qu'elle contient. Ici elle contient `"hello world"` qui est une chaîne de caractères.
    === !!!failure "Erreur"
            ```python linenums="1"
            --8<-- "docs/scripts/python/helloworld/helloworld2"
            ```
            Ici l'erreur est que les guillemets ont été oubliées, et donc, essaye d'écrire la variable `hello` et `world`. Celles-ci n'ayant pas été définies, rien ne ressort du print et le programme plante.
    === !!!failure "Erreur"
            ```python linenums="1"
            --8<-- "docs/scripts/python/helloworld/helloworld3"
            ```
            Ici l'erreur est que les parenthèses ont été oublié, et une fonction en a toujours, l'interpréteur ne comprend donc pas que vient faire ce print devant une chaîne de caractères.

    
