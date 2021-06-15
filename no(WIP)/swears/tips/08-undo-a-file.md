---
tags: tip
title: Helvete da, Jeg må angre endringene mine i en fil! 
id: angre-en-fil
order: 8
---

```git
# finn en hash for en bunt før filen ble endret 
git log
# bruk piltastene for å bla opp og ned i historikken 
# Når du har funnet bunten, lagrer du hash'en 
git checkout [lagret hash] -- sti/til/fil
# den gamle versjonen av filen vil være i indeksen din 
git commit -m "Utrolig, du trenger ikke å kopiere og lime inn for å angre"
```


Da jeg endelig skjønte dette, var det ENORMT. ENORMT. E-N-O-R-M-T. Men alvorlig talt, på hvilken jævla planet er det `checkout --` som den beste måten å angre en fil på? :hever-neven-mot-linus-torvalds: 