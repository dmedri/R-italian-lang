# R-italian-lang

R Italian translations:
- Main focus: R latest stable release;
- external CRAN packages.

## Search for translated labels

If you work on translations, it could be useful search for labels. The script
will do this for you, searching in the main branch and under every available
package.

```
$ ./repo.search restituisce
$ ./repo.search "si utilizza"
```

## Clean the repository

It could happen, if you work with some editors (eg. `poedit`). When you open
a session with a `.po` file, it will try to export a binary file as a test. The
resulting one will be in the same directory with `.mo` extension. To clean up
your source tree, run the following command:

```
$ ./repo.clean
```

## Export archives

At every tag release -- and updates -- it could happen to send translations to
different people. One archive for the R Core Team, to be committed in the
master branch. One archive per-package, to be attached on a mail for
every active package maintainer. The script will create a directory, `archives/`,
to store all `.tgz` files, ready for mailing.

```
$ ./repo.archives
```

## Prepare your translations for Roaster builds

Do you know already the [Roaster](https://github.com/dmedri/roaster)? It's
a recently new project to support R builds (server, standard, virtualenv). One
of its supported special case are virtual environments. This script is made to
add latest updated translations in its source tree, just before any build.

Run:

```
$ ./repo.roaster
```

## Notes for (italian) end-users and developers

If you're using R with the italian language on, your feedback is welcome. To report mistakes or better
translated words/sentence, follow these items:
* open an issue on github (look at the above header bar, at the top of the page);
* fork this repository, apply your changes and request a merge.

---

_Se usate R in lingua italiana, su tutte le piattaforme disponibili, il vostro
resoconto d'utilizzo è molto gradito. Per segnalare errori o traduzioni di frasi
migliori, dovete fare ciò che segue:
* aprire una issue su github (guardate l'intestazione, nella parte in alto della pagina);
* fate un fork del repository, applicate i vostri cambiamenti e richiedete il merge._

## Notes for R translators in other languages

This repository could be easy adapted/used for other languages. With
minor settings will be ready to support your work with a new fashion, the
best choice for this kind of collaborative work. Ask for support.
