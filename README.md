# R-italian-lang

R Italian translations
- Main focus: R release 3.6.3 (latest stable);
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

It could happen, if you work with `poedit. When you open a session with
a .po file, it try to export in binary form as a test. The resulting file
is a .mo file. To clean up your source tree, run the following command:

```
$ ./repo.clean
```

## Create archives for the export

At every tag -- and updates -- it could happen to send translations to
different people. One archive for the R Core Team, to be committed in the
master branch. One archive per-package, to be attached on a mail for
every active package maintainer. The script will create a directory, `archives`,
where there'll be all .tgz file, ready for mailing.

```
$ ./repo.archives
```

## Prepare your translations for Roaster builds

Do you know already the [Roaster](https://github.com/dmedri/roaster)? This
script is made to add latest updated translations in the source tree, just
before any build. It'll do also some validity checks.

```
$ ./repo.roaster
```

## Notes

This repository could be easy adapted and used for other languages. Just
put your .pot/.po file under every '*/po' directory. Ask for help.
