---
tags: tip
title: Faen da, Jeg buntet og kom umiddelbart på at jeg måtte gjøre en liten endring! 
id: Endre-siste-bunt
order: 2
---

```git
# gjør din endring
git add . # eller legg til individuelle filer
git commit --amend --no-edit
# nå innerholder din siste bunt den endringen
# ADVARSEL: Aldri endre på offentlig bunter
```

Dette skjer vanligvis med meg hvis jeg bunter og så tester/linters ... og FML, jeg la ikke mellomrom etter et likhetstegn. Du kan også gjøre endringen som en ny bunt og deretter gjøre `rebase -i` for å mose dem begge sammen, men dette er omtrent en million ganger raskere. 

*Warning: You should never amend commits that have been pushed up to a public/shared branch! Only amend commits that only exist in your local copy or you're gonna have a bad time.*

* Advarsel: Du bør aldri bunten som har blitt dyttet opp til en offentlig/delt gren! Endre bare bunter som finnes i din lokale kopi, ellers vil du ha en dårlig tid. * 