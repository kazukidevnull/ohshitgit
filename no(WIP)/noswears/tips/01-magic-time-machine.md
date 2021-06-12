---
tags: tips
title: pokker da, jeg gjorde noe veldig galt, fortell meg git har en magisk tidsmaskin!?! 
id: magisk tidsmaskin 
order: 1
---

```git
git reflog
# du vil se en liste over alle ting du har
# gjort i git, på tvers av alle grener!
# hver har en indeks HEAD@{index}
# finn den før du brøt alt 
git reset HEAD@{index}
# magisk tidsmaskin 
```


Du kan bruke dette til å få tilbake ting du ved et uhell slettet, eller bare for å fjerne noen ting du prøvde som brøt repo'en, eller for å gjenopprette etter en dårlig sammenslåing, eller bare for å gå tilbake til en tid da ting faktisk fungerte. Jeg bruker `reflog` MYE. stor tipping av hatten til mange mange mange mange mange som foreslo å legge det til! 