# 🐍 Le Python

## Définition

!!!tldr "Définition"
    Le Python est un langage de programmation interprété, multi-paradigme et multiplateformes. Il favorise la programmation impérative structurée, fonctionnelle et orientée objet. Il est doté d'un typage dynamique fort, d'une gestion automatique de la mémoire par ramasse-miettes et d'un système de gestion d'exceptions.
    __*source: Wikipedia[^1]*__
    [^1]: [Wikipedia : Definition](https://fr.wikipedia.org/wiki/Python_(langage))

- [X] Orienté Fonctionelle    
- [X] Orientée Objet

!!!tldr "Info"
    Nous présentons rapidement le pyton afin d'avoir un comparatif avec les langages qui seront présentés après.
## Exemples de codes

### HelloWorld

- Pour commencer, nous allons voir comment écrire `helloworld` dans la console python:

!!!Note "Ecrire `helloworld`"

    === "Code 1"
        !!!Success "Réussite"
            ```python linenums="1"
            --8<-- "docs/scripts/python/helloworld/helloworld1.py"
            ```
            ```pycon
            --8<-- "docs/scripts/python/helloworld/helloworld1console.py"
            ```
            Voici comment écrire `helloworld` dans la console. La fonction `print` sert à écrire dans la console ce qu'elle contient. Ici elle contient `"hello world"` qui est une chaîne de caractères.
            
    === "Code 2"
        !!!failure "Erreur"
            ```python linenums="1" hl_lines="1"
            --8<-- "docs/scripts/python/helloworld/helloworld2.py"
            ```
            ```pycon
            --8<-- "docs/scripts/python/helloworld/helloworld2console.py"
            ```
            Ici l'erreur est que les guillemets ont été oubliées, et donc, essaye d'écrire la variable `hello` et `world`. Celles-ci n'ayant pas été définies, rien ne ressort du print et le programme plante.

    === "Code 3"
        !!!failure "Erreur"
            ```python linenums="1" hl_lines="1"
            --8<-- "docs/scripts/python/helloworld/helloworld3.py"
            ```
            ```pycon
            --8<-- "docs/scripts/python/helloworld/helloworld3console.py"
            ```
            Ici l'erreur est que les parenthèses ont été oublié, et une fonction en a toujours, l'interpréteur ne comprend donc pas que vient faire ce print devant une chaîne de caractères.

### Boucles
    
- Ici, nous allons voir comment faire une boucle qui envoi dans la console les chiffres de 0 à 10 inclus.

!!!Note "Les boucles"

    === "Code 1"
        !!!Success "Réussite"
            ```python linenums="1"
            --8<-- "docs/scripts/python/boucles/boucle1.py"
            ```
            ```pycon
            --8<-- "docs/scripts/python/boucles/boucle1console.py"
            ```
            Voici comment est faite une boucle en python. Elle permet donc d'écrire dans une boucle de 10 tours, les chiffres de 0 à 11 exclus.
    
    === "Code 2"
        !!!Success "Réussite"
            ```python linenums="1"
            --8<-- "docs/scripts/python/boucles/boucle2.py"
            ```
            ```pycon
            --8<-- "docs/scripts/python/boucles/boucle2console.py"
            ```
            Voici un deuxième façon, moins optimisé, car si il y a 1000 chiffres, il faut tous les écrire à la main, mais cela fonctionne.

    === "Code 3"
        !!!failure "Erreur"
            ```python linenums="1" hl_lines="2"
            --8<-- "docs/scripts/python/boucles/boucle3.py"
            ```
            ```pycon
            --8<-- "docs/scripts/python/boucles/boucle3console.py"
            ```
            Ici l'erreur est que le nom de la variable de la boucle n'est pas la même que celle dans le print, donc la variable n'existe même pas.

### Mathématiques

!!!note "Mathématiques"
    python est aussi un outils permettant de faire des mathématiques, il peut être parfois plus simple, d'utiliser python pour des formules répétitives, afin de réaliser instantanément les calculs.

- Ici nous allons voir comment transformer cette formule en un code python, qui nous renverras le résulat dans la console

$$
\Delta = b^2-4ac
$$

> Cette formule permet de calculer Delta

!!!Note "Mathématiques"

    === "Code 1"
        !!!Success "Réussite"
            ```python linenums="1"
            --8<-- "docs/scripts/python/delta/delta1.py"
            ```
            ```pycon
            --8<-- "docs/scripts/python/delta/delta1console.py"
            ```
            Voici ici la manière la plus simple de calculer un Delta, pour changer les valeurs, il suffira de changer les valeurs de "a", "b" et "c", ou de mettre un `int(input())` afin de demander à l'utilisateur du script quelles sont les valeurs que veux l'utilisateur pour effectuer le calcul.
    
    === "Code 2"
        !!!Success "Réussite"
            ```python linenums="1"
            --8<-- "docs/scripts/python/delta/delta2.py"
            ```
            ```pycon
            --8<-- "docs/scripts/python/delta/delta2console.py"
            ```
            Voici une deuxième façon de calculer Delta, mais elle n'est valable que pour 1 seul calcul, sinon il faut modifier les éléments dans print. Alors que le premier peut vite s'adapter avec des entrées utilisateurs en changeant la valeur de chaque variables.

    === "Code 3"
        !!!failure "Erreur"
            ```python linenums="1" hl_lines="2"
            --8<-- "docs/scripts/python/delta/delta3.py"
            ```
            ```pycon
            --8<-- "docs/scripts/python/delta/delta3console.py"
            ```
            Ici l'erreur est que les variables "a", "b" et "c" ne sont pas initialisées, et donc le print ne peux pas écrire le résultat demandé.

