---
tags: tip
title: pokker, Jeg må angre en bunt fra for 5 bunter tilbake! 
id: angre-en-bunt
order: 7
---

```git
# finn bunten du ønsker å angre
git log
# bruk piltastene for å bla opp og ned i historikken 
# Når du har funnet bunten, lagrer du bunt hash'en 
git revert [lim in bunt hash'en]
# git will create a new commit that undoes that commit git vil opprette en ny bunt som angrer den bunten
# følg instruksjonene for å redigere bunt meldingen 
# eller bare lagre og bunt
```

Det viser seg at du ikke trenger å spore og kopiere og lime inn det gamle filinnholdet i den eksisterende filen for å angre endringene! Hvis du har begått en feil, kan du angre bunten alt på en gang med `revert`. 

Du kan også tilbakestille en enkelt fil i stedet for hele bunten! Men selvfølgelig, på ekte git-måte, er det et helt annet sett med kommander...