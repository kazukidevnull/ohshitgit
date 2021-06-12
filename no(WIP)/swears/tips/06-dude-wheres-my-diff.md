---
tags: tip
title: Faen da, Jeg prøvde å gjøre en diff, men ingenting skjedde?!
id: hei-hvor-er-min-diff
order: 6
---

If you know that you made changes to files, but `diff` is empty, you probably `add`-ed your files to staging and you need to use a special flag.
Hvis du vet at du har gjort endringer til filene, men `diff` er tom, har du sannsynligvis `add` filene dine til `staging`, og du må bruke et spesielt flagg. 
```git
git diff --staged
```

Filer under &macr;\\\_(ツ)\_/&macr; (ja, jeg vet at dette er en funksjon, ikke en feil, men det er jævla forvirrende og ikke åpenbart første gang det skjer med deg!)


