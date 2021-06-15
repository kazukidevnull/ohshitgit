---
tags: tip
title: helvete med dette støyet, jeg gir opp. 
id: helvete-med-dette-støyet
notat: dette skal alltid være den siste i listen, så satt rekkefølgen til 20 slik at jeg ikke trenger å endre navn/rekkefølgen på den
order: 20
---

```git
cd ..
sudo rm -r faen-git-repo-mappen
git clone https://noen.github.url/faen-git-repo-mappen.git
cd faen-git-repo-mappen
```

Takk til Eric V. for denne. Alle klager på bruken av `sudo` i denne vitsen kan rettes til ham. 


Men seriøst, hvis din gren er sååå på tryne at du trenger å tilbakestille tilstanden i mappen din for å være den samme som den eksterne mappen på en "git-godkjent" måte, prøv dette, men pass på at dette er destruktive og uopprettelige handlinger! 

```git
# få den siste opprinnelsetilstanden
git fetch origin
git checkout master
git reset --hard origin/master
# slett usporete filer og mapper 
git clean -d --force
# gjenta "checkout/reset/clean" for hver gren som er på tryne
```