---
tags: tip
title: pokker, Jeg bunted ved et uhell til master som skulle ha vært på en helt ny gren! 
id: buntet-til-hovedgren-med-uhell
order: 4
---

```git
# opprette en ny gren fra gjeldende tilstand av hovedgrenen 
git branch some-new-branch-name
# fjern siste bunt fra hovedgrenen 
git reset HEAD~ --hard
git checkout some-new-branch-name
# din bunt lever no i denne gren :)
```

Merk: dette fungerer ikke hvis du allerede har dyttet bunten til en offentlig/delt gren, og hvis du først har prøvd andre ting, må du kanskje `git reset HEAD@ {nummer av bunter bak` i stedet av `HEAD ~`. Uendelig tristhet. Også, mange mange mange mennesker foreslo en fantastisk måte å gjøre dette kortere som jeg ikke kjente selv. Takk alle sammen!


