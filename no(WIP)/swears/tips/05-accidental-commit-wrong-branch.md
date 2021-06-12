---
tags: tip
title: Faen da, Jeg buntet til feil gren med et uhell
id: uheldigvis-buntet-feil-gren
order: 5
---

```git
# angre den siste bunt, men la endringene være tilgjengelig
git reset HEAD~ --soft
git stash
# flytt til riktig gren
git checkout navn-på-riktig-gren 
git stash pop
git add . # eller legg til individuelle filer 
git commit -m "din melding her";
# nå er endringene dine på riktig gren
```

Mange folk har foreslått å bruke `cherry-pick` for denne situasjonen også, så velg det som gir mest mening for deg! 

```git
git checkout navn-på-riktig-gren 
# hent den siste bunt til hovedgren
git cherry-pick master
# slett den fra hovedgren
git checkout master
git reset HEAD~ --hard
```