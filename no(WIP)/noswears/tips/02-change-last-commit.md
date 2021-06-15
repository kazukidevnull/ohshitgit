---
tags: tip
title: Pokker, Jeg buntet og kom umiddelbart på at jeg måtte gjøre en liten endring! 
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

Dette skjer vanligvis med meg hvis jeg bunter og så tester/linters ... og stønn, jeg la ikke mellomrom etter et likhetstegn. Du kan også gjøre endringen som en ny bunt og deretter gjøre `rebase -i` for å mose dem begge sammen, men dette er omtrent en million ganger raskere. 

* Advarsel: Du bør aldri endre bunter som har blitt dyttet opp til en offentlig/delt gren! Endre bare bunter som finnes i din lokale kopi, ellers vil du ha en dårlig tid. * 