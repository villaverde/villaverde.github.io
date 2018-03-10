.. title: Git - Deshaciendo la preparación de un archivo antes de hacer commit
.. slug: git-deshaciendo-la-preparacion-de-un-archivo-antes-de-hacer-commit
.. date: 2015-04-23 22:53:33 UTC+01:00
.. tags: Git
.. category: Programación
.. link:
.. description:
.. type: text

.. image:: /imgpost/git.png

Cuando por error añadimos un archivo al área de preparación para hacer un comiit podemos quitarlo con reset HEAD archivo

Pongo un ejemplo

.. code-block:: shell

  $ git add readme.txt

  $ git status

  # On branch master

  # Changes not staged for commit:

  # (use "git reset HEAD <file>..." to unstage)

  #

  #    modified:   readme.txt

  #
