---
title: 'Outgroup Intolerance and Support for Democracy: An Analysis of White Americans in the World Values Survey Data'
author: steve
layout: post
date: "2017-08-18"
permalink:
categories:
  - Political Science
excerpt: "World Values Survey data suggest outgroup intolerance and bigotry in the United States also coincide with lukewarm attitudes about democracy."
---


{% include image.html url="/images/charlottesville-white-pride-rally.jpg" caption="A man marching with white nationalists makes a slashing motion across his throat toward counter-protester in Charlottesville's white pride rally. (Chip Somodevilla/Getty Images)" width=400 align="right" %}

Last weekend's events in Charlottesville, Virginia, along with the ongoing reaction from President Trump and complicit acceptance of these developments by Republican leadership, suggest a troubling trend emerging in American politics. Racism has always been a fact of life in American politics. It's also been a recurring theme of Republican politics for the past 50 years (e.g. Nixon's ["law and order,"](https://twitter.com/AdamSerwer/status/857626382620295168) Reagan's ["welfare queen,"](http://www.npr.org/sections/codeswitch/2013/12/20/255819681/the-truth-behind-the-lies-of-the-original-welfare-queen) Bush's Horton ad) despite the Chair of the Republican National Committee [trying to pretend racism hasn't been an important calling card](https://twitter.com/stevenvmiller/status/897918796605906944) for the GOP.

Racism has always been a fact of American politics, and perhaps no candidate had [ever raised subtext to text like Trump](http://svmiller.com/blog/2017/04/age-income-racism-partisanship-trump-vote-2016/). My worries run deeper than that. Watch [the *Vice* documentary on Charlottesville](https://news.vice.com/story/vice-news-tonight-full-episode-charlottesville-race-and-terror) where these white supremacists advertise they *want* to fight and subvert the public order. Look at the photos of the white supremacists and their supporters armed to the teeth and, [per Virginia's governor](https://www.nytimes.com/2017/08/13/us/charlottesville-protests-white-nationalists.html?_r=0), effectively outflanking the police (i.e. the monopoly on the legitimate use of force in this context, per Max Weber). Think of the racial overtones in defense of a slave-holding secessionist regime that fought a war against the United States. Trump's press conference at his residence and subsequent Twitter tantrums seem to suggest a tenuous commitment to democratic principles for those 1) taking part in these protests and 2) supporting these rallies/intimidation measures.

Four waves of World Values Survey (WVS) data from 1995 to 2011 largely support that. White respondents in the United States over those four waves who expressed that they would not like to have various outgroups of interest as neighbors (i.e. those from a different race, Muslims, immigrants/foreign workers, Jews, and those speaking a different language) were more likely to support rule of government by a strong leader without legislative or electoral oversight, rule of government by the army, and were more likely to oppose democracy, in general. I detail the method and the analysis below.


```
## Error in library(mirt): there is no package called 'mirt'
```

```
## Error in library(stevemisc): there is no package called 'stevemisc'
```

```
## Error in library(merTools): there is no package called 'merTools'
```

```
## Error: '~/Dropbox/data/wvs/wvs-usa-wave3-6.csv' does not exist.
```

```
## Error in tolower(names(USA)): objeto 'USA' no encontrado
```

```
## Error in nrow(USA): objeto 'USA' no encontrado
```

```
## Error in eval(expr, envir, enclos): objeto 'USA' no encontrado
```

```
## Error in eval(expr, envir, enclos): objeto 'USA' no encontrado
```

```
## Error in eval(expr, envir, enclos): objeto 'USA' no encontrado
```

```
## Error in eval(expr, envir, enclos): objeto 'USA' no encontrado
```

```
## Error in with(USA, ifelse(region == -2, NA, region)): objeto 'USA' no encontrado
```

```
## Error in with(USA, region - 840000): objeto 'USA' no encontrado
```

```
## Error in eval(expr, envir, enclos): objeto 'USA' no encontrado
```

```
## Error in with(USA, ifelse(censusd >= 9, 9, censusd)): objeto 'USA' no encontrado
```

```
## Error in USA$censusd[USA$censusd == 1] <- "New England": objeto 'USA' no encontrado
```

```
## Error in USA$censusd[USA$censusd == 2] <- "Middle Atlantic": objeto 'USA' no encontrado
```

```
## Error in USA$censusd[USA$censusd == 3] <- "South Atlantic": objeto 'USA' no encontrado
```

```
## Error in USA$censusd[USA$censusd == 4] <- "East South Central": objeto 'USA' no encontrado
```

```
## Error in USA$censusd[USA$censusd == 5] <- "West South Central": objeto 'USA' no encontrado
```

```
## Error in USA$censusd[USA$censusd == 6] <- "East North Central": objeto 'USA' no encontrado
```

```
## Error in USA$censusd[USA$censusd == 7] <- "West North Central": objeto 'USA' no encontrado
```

```
## Error in USA$censusd[USA$censusd == 8] <- "Mountain": objeto 'USA' no encontrado
```

```
## Error in USA$censusd[USA$censusd == 9] <- "Pacific": objeto 'USA' no encontrado
```

```
## Error in eval(expr, envir, enclos): objeto 'USA' no encontrado
```

```
## Error in with(USA, ifelse(censusr >= 9, 9, censusr)): objeto 'USA' no encontrado
```

```
## Error in USA$censusr[USA$censusr == 1 | USA$censusr == 2] <- "Northeast": objeto 'USA' no encontrado
```

```
## Error in USA$censusr[USA$censusr == 6 | USA$censusr == 7] <- "Midwest": objeto 'USA' no encontrado
```

```
## Error in USA$censusr[USA$censusr == 3 | USA$censusr == 4 | USA$censusr == : objeto 'USA' no encontrado
```

```
## Error in USA$censusr[USA$censusr == 8 | USA$censusr == 9] <- "West": objeto 'USA' no encontrado
```

```
## Error in eval(expr, envir, enclos): objeto 'USA' no encontrado
```

```
## Error in with(USA, ifelse(raceethnic == -2, NA, raceethnic)): objeto 'USA' no encontrado
```

```
## Error in USA$raceethnic[USA$x051 == 200] <- "Black": objeto 'USA' no encontrado
```

```
## Error in USA$raceethnic[USA$x051 == 1250] <- "Hispanic": objeto 'USA' no encontrado
```

```
## Error in USA$raceethnic[USA$x051 == 1400] <- "White": objeto 'USA' no encontrado
```

```
## Error in USA$raceethnic[USA$x051 == 8000] <- "Other": objeto 'USA' no encontrado
```

```
## Error in USA$raceethnic[USA$x051 == 8001] <- "Mixed Race": objeto 'USA' no encontrado
```

```
## Error in USA$raceethnic[USA$x051 == 840002] <- "White": objeto 'USA' no encontrado
```

```
## Error in USA$raceethnic[USA$x051 == 840003] <- "Black": objeto 'USA' no encontrado
```

```
## Error in USA$raceethnic[USA$x051 == 840004] <- "Other": objeto 'USA' no encontrado
```

```
## Error in USA$raceethnic[USA$x051 == 840005] <- "Hispanic": objeto 'USA' no encontrado
```

```
## Error in USA$raceethnic[USA$x051 == 840006] <- "Mixed Race": objeto 'USA' no encontrado
```

```
## Error in USA$raceethnic[USA$x051 == 840007] <- "Other": objeto 'USA' no encontrado
```

```
## Error in USA$raceethnic[USA$x051 == 840008] <- "Other": objeto 'USA' no encontrado
```

```
## Error in USA$raceethnic[USA$x051 == 840009] <- "Other": objeto 'USA' no encontrado
```

```
## Error in USA$raceethnic[USA$x051 == 840010] <- "White": objeto 'USA' no encontrado
```

```
## Error in USA$raceethnic[USA$x051 == 840011] <- "Black": objeto 'USA' no encontrado
```

```
## Error in USA$raceethnic[USA$x051 == 840012] <- "Hispanic": objeto 'USA' no encontrado
```

```
## Error in with(USA, ifelse(raceethnic == "White", 1, 0)): objeto 'USA' no encontrado
```

```
## Error in with(USA, ifelse(raceethnic == "Black", 1, 0)): objeto 'USA' no encontrado
```

```
## Error in with(USA, ifelse(raceethnic == "Hispanic", 1, 0)): objeto 'USA' no encontrado
```

```
## Error in USA$party <- NA: objeto 'USA' no encontrado
```

```
## Error in USA$party[USA$e179wvs == 5] <- "Other": objeto 'USA' no encontrado
```

```
## Error in USA$party[USA$e179wvs == 840001] <- "Republican": objeto 'USA' no encontrado
```

```
## Error in USA$party[USA$e179wvs == 840002] <- "Democrat": objeto 'USA' no encontrado
```

```
## Error in USA$party[USA$e179wvs == 840003] <- "Independent": objeto 'USA' no encontrado
```

```
## Error in USA$party[USA$e179wvs == 840004] <- "Libertarian": objeto 'USA' no encontrado
```

```
## Error in USA$party[USA$e179wvs == 840005] <- "Reform": objeto 'USA' no encontrado
```

```
## Error in with(USA, ifelse(party == "Republican", 1, 0)): objeto 'USA' no encontrado
```

```
## Error in with(USA, ifelse(party == "Democrat", 1, 0)): objeto 'USA' no encontrado
```

```
## Error in with(USA, recode(e114, "-5:-1=NA; 1=4; 2=3; 3=2; 4=1")): objeto 'USA' no encontrado
```

```
## Error in with(USA, recode(e115, "-5:-1=NA; 1=4; 2=3; 3=2; 4=1")): objeto 'USA' no encontrado
```

```
## Error in with(USA, recode(e116, "-5:-1=NA; 1=4; 2=3; 3=2; 4=1")): objeto 'USA' no encontrado
```

```
## Error in with(USA, recode(e117, "-5:-1=NA; 1=4; 2=3; 3=2; 4=1")): objeto 'USA' no encontrado
```

```
## Error in with(USA, recode(e224, "-5:-1=NA")): objeto 'USA' no encontrado
```

```
## Error in with(USA, recode(e225, "-5:-1=NA")): objeto 'USA' no encontrado
```

```
## Error in with(USA, recode(e226, "-5:-1=NA")): objeto 'USA' no encontrado
```

```
## Error in with(USA, recode(e227, "-5:-1=NA")): objeto 'USA' no encontrado
```

```
## Error in with(USA, recode(e228, "-5:-1=NA")): objeto 'USA' no encontrado
```

```
## Error in with(USA, recode(e229, "-5:-1=NA")): objeto 'USA' no encontrado
```

```
## Error in with(USA, recode(e230, "-5:-1=NA")): objeto 'USA' no encontrado
```

```
## Error in with(USA, recode(e231, "-5:-1=NA")): objeto 'USA' no encontrado
```

```
## Error in with(USA, recode(e232, "-5:-1=NA")): objeto 'USA' no encontrado
```

```
## Error in with(USA, recode(e233, "-5:-1=NA")): objeto 'USA' no encontrado
```

```
## Error in with(USA, recode(e234, "-5:-1=NA")): objeto 'USA' no encontrado
```

```
## Error in with(USA, recode(e235, "-5:-1=NA")): objeto 'USA' no encontrado
```

```
## Error in with(USA, recode(e236, "-5:-1=NA")): objeto 'USA' no encontrado
```

```
## Error in with(USA, recode(x003, "-5:-1=NA")): objeto 'USA' no encontrado
```

```
## Error in with(USA, recode(x001, "-5:-1=NA; 1=0; 2=1")): objeto 'USA' no encontrado
```

```
## Error in with(USA, recode(x028, "-5:-1=NA; 1:6=0; 7=1; 8=0")): objeto 'USA' no encontrado
```

```
## Error in with(USA, ifelse(c006 < 0, NA, c006 - 1)): objeto 'USA' no encontrado
```

```
## Error in with(USA, ifelse(e033 < 0, NA, e033 - 1)): objeto 'USA' no encontrado
```

```
## Error in with(USA, recode(x045, "-5:-1=NA; 1=4; 2=3; 3=2; 4=1; 5=0")): objeto 'USA' no encontrado
```

```
## Error in with(USA, ifelse(x047 < 0, NA, x047 - 1)): objeto 'USA' no encontrado
```

```
## Error in with(USA, recode(x025, "-5:-1=NA")): objeto 'USA' no encontrado
```

```
## Error in with(USA, recode(x025, "-5:-1=NA; 1:6=1; 7:8=0")): objeto 'USA' no encontrado
```

```
## Error in with(USA, recode(x025, "-5:-1=NA; 1:3=1; 4:8=0")): objeto 'USA' no encontrado
```

```
## Error in with(USA, recode(x025, "-5:-1=NA; 1:7=0; 8=1")): objeto 'USA' no encontrado
```

```
## Error in USA$educatr <- NA: objeto 'USA' no encontrado
```

```
## Error in with(USA, ifelse((educat >= 1 & educat <= 3) | educat == 5, "Did not finish HS", : objeto 'USA' no encontrado
```

```
## Error in with(USA, ifelse(educat == 4 | educat == 6, "HS grad", educatr)): objeto 'USA' no encontrado
```

```
## Error in with(USA, ifelse(educat == 7, "Some college", educatr)): objeto 'USA' no encontrado
```

```
## Error in with(USA, ifelse(educat == 8, "College educated", educatr)): objeto 'USA' no encontrado
```

```
## Error in eval(expr, envir, enclos): objeto 'USA' no encontrado
```

```
## Error in with(USA, recode(y021, "-5:-1=NA")): objeto 'USA' no encontrado
```

```
## Error in with(USA, recode(y022, "-5:-1=NA")): objeto 'USA' no encontrado
```

```
## Error in with(USA, recode(y023, "-5:-1=NA")): objeto 'USA' no encontrado
```

```
## Error in with(USA, recode(y024, "-5:-1=NA")): objeto 'USA' no encontrado
```

```
## Error in with(USA, data.frame(uid, autonomy, a029, a034, a042)): objeto 'USA' no encontrado
```

```
## Error in lapply(X = X, FUN = FUN, ...): objeto 'Autonomy' no encontrado
```

```
## Error in with(Autonomy, ifelse(is.na(a029) & is.na(a034) & is.na(a042), : objeto 'Autonomy' no encontrado
```

```
## Error in subset(Autonomy, removeme == 0): objeto 'Autonomy' no encontrado
```

```
## Error in Autonomy$removeme <- NULL: objeto 'Autonomy' no encontrado
```

```
## Error in colnames(Autonomy) <- c("uid", "autonomy", "kid_ind", "kid_imag", : objeto 'Autonomy' no encontrado
```

```
## Error in with(Autonomy, recode(kid_obed, "1=0;0=1")): objeto 'Autonomy' no encontrado
```

```
## Error in mirt(Autonomy[, 3:ncol(Autonomy)], model = 1, itemtype = "graded", : no se pudo encontrar la función "mirt"
```

```
## Error in fscores(AutM, full.scores = TRUE, full.scores.SE = TRUE): no se pudo encontrar la función "fscores"
```

```
## Error in cbind(Autonomy, autscores): objeto 'Autonomy' no encontrado
```

```
## Error in revalue(names(x), replace, warn_missing = warn_missing): objeto 'Autonomy' no encontrado
```

```
## Error in with(Autonomy, cor(laut, autonomy, use = "complete.obs")): objeto 'Autonomy' no encontrado
```

```
## Error in rbind.fill(x[by], y[by]): objeto 'USA' no encontrado
```

```
## Error in with(USA, data.frame(uid, equality, c001, d059, d060)): objeto 'USA' no encontrado
```

```
## Error in lapply(X = X, FUN = FUN, ...): objeto 'Equality' no encontrado
```

```
## Error in with(Equality, ifelse(is.na(c001) & is.na(d059) & is.na(d060), : objeto 'Equality' no encontrado
```

```
## Error in subset(Equality, removeme == 0): objeto 'Equality' no encontrado
```

```
## Error in Equality$removeme <- NULL: objeto 'Equality' no encontrado
```

```
## Error in colnames(Equality) <- c("uid", "equality", "menjob", "menleaders", : objeto 'Equality' no encontrado
```

```
## Error in mirt(Equality[, 3:ncol(Equality)], model = 1, itemtype = "graded", : no se pudo encontrar la función "mirt"
```

```
## Error in fscores(EquM, full.scores = TRUE, full.scores.SE = TRUE): no se pudo encontrar la función "fscores"
```

```
## Error in cbind(Equality, equscores): objeto 'Equality' no encontrado
```

```
## Error in revalue(names(x), replace, warn_missing = warn_missing): objeto 'Equality' no encontrado
```

```
## Error in with(Equality, cor(lequ, equality, use = "complete.obs")): objeto 'Equality' no encontrado
```

```
## Error in rbind.fill(x[by], y[by]): objeto 'USA' no encontrado
```

```
## Error in with(USA, data.frame(uid, choice, f118, f120, f121)): objeto 'USA' no encontrado
```

```
## Error in lapply(X = X, FUN = FUN, ...): objeto 'Choice' no encontrado
```

```
## Error in with(Choice, ifelse(is.na(f118) & is.na(f120) & is.na(f121), : objeto 'Choice' no encontrado
```

```
## Error in subset(Choice, removeme == 0): objeto 'Choice' no encontrado
```

```
## Error in Choice$removeme <- NULL: objeto 'Choice' no encontrado
```

```
## Error in colnames(Choice) <- c("uid", "choice", "hj", "aj", "dj"): objeto 'Choice' no encontrado
```

```
## Error in mirt(Choice[, 3:ncol(Choice)], model = 1, itemtype = "graded", : no se pudo encontrar la función "mirt"
```

```
## Error in fscores(ChoM, full.scores = TRUE, full.scores.SE = TRUE): no se pudo encontrar la función "fscores"
```

```
## Error in cbind(Choice, choscores): objeto 'Choice' no encontrado
```

```
## Error in revalue(names(x), replace, warn_missing = warn_missing): objeto 'Choice' no encontrado
```

```
## Error in with(Choice, cor(lcho, choice, use = "complete.obs")): objeto 'Choice' no encontrado
```

```
## Error in rbind.fill(x[by], y[by]): objeto 'USA' no encontrado
```

```
## Error in with(USA, data.frame(uid, voice, e001, e002, e003, e004)): objeto 'USA' no encontrado
```

```
## Error in lapply(X = X, FUN = FUN, ...): objeto 'Voice' no encontrado
```

```
## Error in Voice$acsay <- NA: objeto 'Voice' no encontrado
```

```
## Error in with(Voice, ifelse(e001 == 3, 2, acsay)): objeto 'Voice' no encontrado
```

```
## Error in with(Voice, ifelse(e002 == 3, 1, acsay)): objeto 'Voice' no encontrado
```

```
## Error in with(Voice, ifelse(e001 != 3 & e002 != 3 & !is.na(e001), 0, acsay)): objeto 'Voice' no encontrado
```

```
## Error in Voice$apsay <- NA: objeto 'Voice' no encontrado
```

```
## Error in with(Voice, ifelse((e003 == 2 & e004 == 4) | (e003 == 4 & e004 == : objeto 'Voice' no encontrado
```

```
## Error in with(Voice, ifelse((e003 == 2 & e004 != 4) | (e003 == 4 & e004 != : objeto 'Voice' no encontrado
```

```
## Error in with(Voice, ifelse((e003 != 2 & e004 == 4) | (e003 != 4 & e004 == : objeto 'Voice' no encontrado
```

```
## Error in with(Voice, ifelse((e003 != 2 & e004 != 4) & (e003 != 4 & e004 != : objeto 'Voice' no encontrado
```

```
## Error in with(Voice, ifelse(is.na(acsay) & is.na(apsay), 1, 0)): objeto 'Voice' no encontrado
```

```
## Error in subset(Voice, removeme == 0): objeto 'Voice' no encontrado
```

```
## Error in Voice$removeme <- NULL: objeto 'Voice' no encontrado
```

```
## Error in mirt(Voice[, 7:ncol(Voice)], model = 1, itemtype = "graded", : no se pudo encontrar la función "mirt"
```

```
## Error in fscores(VoiM, full.scores = TRUE, full.scores.SE = TRUE): no se pudo encontrar la función "fscores"
```

```
## Error in cbind(Voice, voiscores): objeto 'Voice' no encontrado
```

```
## Error in revalue(names(x), replace, warn_missing = warn_missing): objeto 'Voice' no encontrado
```

```
## Error in with(Voice, cor(lvoi, voice, use = "complete.obs")): objeto 'Voice' no encontrado
```

```
## Error in rbind.fill(x[by], y[by]): objeto 'USA' no encontrado
```

```
## Error in with(USA, data.frame(uid, emancvalues, laut, lequ, lcho, lvoi)): objeto 'USA' no encontrado
```

```
## Error in with(Emanc, (1/4) * (laut + lequ + lcho + lvoi)): objeto 'Emanc' no encontrado
```

```
## Error in with(Emanc, cor(emancvalues, lemanc, use = "complete.obs")): objeto 'Emanc' no encontrado
```

```
## Error in is.data.frame(data): objeto 'Emanc' no encontrado
```

```
## Error in is.data.frame(data): objeto 'Emanc' no encontrado
```

```
## Error in is.data.frame(data): objeto 'Emanc' no encontrado
```

```
## Error in is.data.frame(data): objeto 'Emanc' no encontrado
```

```
## Error in tidy(A1): objeto 'A1' no encontrado
```

```
## Error in tidy(A2): objeto 'A2' no encontrado
```

```
## Error in tidy(A3): objeto 'A3' no encontrado
```

```
## Error in tidy(A4): objeto 'A4' no encontrado
```

```
## Error in with(Emanc, ifelse(is.na(laut) & is.na(lemanc), A1df[1, 2] + : objeto 'Emanc' no encontrado
```

```
## Error in with(Emanc, ifelse(is.na(lequ) & is.na(lemanc), A2df[1, 2] + : objeto 'Emanc' no encontrado
```

```
## Error in with(Emanc, ifelse(is.na(lcho) & is.na(lemanc), A3df[1, 2] + : objeto 'Emanc' no encontrado
```

```
## Error in with(Emanc, ifelse(is.na(lvoi) & is.na(lemanc), A4df[1, 2] + : objeto 'Emanc' no encontrado
```

```
## Error in with(Emanc, data.frame(uid, lemanc)): objeto 'Emanc' no encontrado
```

```
## Error in rbind.fill(x[by], y[by]): objeto 'USA' no encontrado
```

```
## Error in eval(lhs, parent, parent): objeto 'USA' no encontrado
```

```
## Error in eval(lhs, parent, parent): objeto 'USA' no encontrado
```

```
## Error in lapply(X = X, FUN = FUN, ...): objeto 'Neighb' no encontrado
```

```
## Error in eval(lhs, parent, parent): objeto 'Neighb' no encontrado
```

```
## Error in eval(lhs, parent, parent): objeto 'Neighb' no encontrado
```

```
## Error in lapply(X = X, FUN = FUN, ...): objeto 'Neighb' no encontrado
```

```
## Error in left_join(USA, Neighb): objeto 'USA' no encontrado
```

```
## Error in eval(lhs, parent, parent): objeto 'USA' no encontrado
```

```
## Error in eval(lhs, parent, parent): objeto 'USA' no encontrado
```


## The Data

I use the aforementioned four waves of WVS data for this analysis and pattern the analysis off what I did in last year's post about how Trump is picking up on what I termed [a "strong leader problem" in the U.S.](http://svmiller.com/blog/2016/05/america-strong-leaders-world-values-survey-trump/). Much of that analysis became [this article](http://svmiller.com/research/economic-threats-or-societal-turmoil-understanding-preferences-for-authoritarian-political-systems/) now [in print at *Political Behavior*](http://link.springer.com/article/10.1007/s11109-016-9363-7?wt_mc=Affiliate.CommissionJunction.3.EPR1089.DeepLink).

Briefly, I take various general questions about attitudes toward democracy for Americans readily available in the WVS and regress them on some variables of interest. These dependent variables are four-item measures about whether the responsdent would think having a strong leader without legislative or electoral oversight or rule of government by the army would be good for the United States. I also include whether the respondent believes having a democracy would be good for the United States. I condense these four-item measures to equal 1 if the respondent thinks a strong leader or army rule would be good and if having democracy would be bad. I invert the scale of the democracy question for comparability of coefficients.

I simplify the set of regressors to variables for age, age-squared, whether the respondent is a woman, whether the respondent has a high school education or less, the respondent's ideology, ideology-squared, an income scale measuring personal income, whether the respondent identifies as a Republican or Democrat relative to a baseline of independents or third-party supporters (e.g. Libertarians, Reform Party [remember them?]), whether the respondent is unemployed, and [the emancipative values measure from Welzel](http://www.cambridge.org/us/academic/subjects/politics-international-relations/comparative-politics/freedom-rising-human-empowerment-and-quest-emancipation?format=PB&isbn=9781107664838).

I offer one new variable here to measure white intolerance for various outgroups that routinely appear as pejoratives for the white supremacists like we saw in Charlottesville. The WVS is not perfect for these questions. Indeed, eliciting a xenophobic or racist statement in a survey or survey experiment is *hard* (see: [my summary](http://svmiller.com/blog/2017/04/age-income-racism-partisanship-trump-vote-2016/) of what [Christopher DeSante](http://pages.iu.edu/~cdesante/) and [Candis Smith](http://publicpolicy.unc.edu/people/candis-w-smith/) are doing) and typically require more nuance than WVS shows (e.g. [endorsement experiments](https://imai.princeton.edu/research/support.html)). Still, WVS uses something close to a familiar device for intolerance researchers. The survey asks respondents to say what types of people they would not like to have as neighbors.[^social] The respondent can name any they like from a set list of familiar groups. 

[^social]: In essence, this variable is a measure for "social intolerance" rather than "political intolerance" for those aware of the distinction.

This question has evolved over time and is generalizable to different countries and contexts in WVS. Available responses in the U.S. include:

- Criminals
- Members of a different race
- Heavy drinkers
- Emotionally unstable people
- Muslims
- Immigrants/foreign workers
- People with AIDS
- Drug addicts
- Homosexuals
- Jews
- People of a different religion
- People of the same religion
- "Militant minority"
- Political extremists
- Unmarried couples living together
- People who speak a different language

There is substantial variety in this question. There are also a few "easy" targets here, like criminals, heavy drinkers, and drug addicts. While I'm sure these items have important subtext to which a respondent might react (e.g. "criminals"), they're banal without it. Indeed, most respondents selected these groups of all the available options because they probably make crummy neighbors.

I'm most interested in those who say that they would not want members of a different race, Muslims, immigrants/foreign workers, Jews, and those who speak a different language as neighbors. White supremacists/nationalists and nativists routinely single out these groups in one form or another, with varying levels of subtext. I code a dummy that equals 1 if a respondent identified any one of those as an unwelcome neighbor.[^militant] 

[^militant]: I could just as well included "militant minority" but I have a few misgivings with this option. One, it's loaded. I may not object to a "minority" as neighbor, but "militant?" Who wants that? Further, WVS provides no other documentation about what they mean here.

Unlike last year's post on the strong leader problem, I subset the data to just white respondents. The models that follow are mixed effects logistic models with random effects for the condensed Census region, the year of the survey, and the Census-year (e.g. "South-1995", "Northeast-2011").

## The Results

The three regressions I summarize in Table 1 all suggest a positive effect of white intolerance toward these outgroups on a general opposition to democracy. Respondents who would not want members of a different race, Muslims, immigrants/foreign workers, Jews, and those who speak a different language as neighbors were more likely to want rule of government by a strong leader, the army, or were more likely to oppose democracy relative to respondents who did not signal an opposition to any of these outgroups as neighbors (i.e. those who would not want criminals or unmarried couples instead).

Interestingly, the only other effect that is positive and robust across all three models is the education variable. Those with a high school education or less were more likely to want a strong leader or the army to rule the government. They were also more likely to oppose democracy as a political system for the United States. 

<center>

```
## Error in checkFormulaData(formula, data, checkLHS = control$check.formula.LHS == : bad 'data': objeto 'USA' no encontrado
```

```
## Error in checkFormulaData(formula, data, checkLHS = control$check.formula.LHS == : bad 'data': objeto 'USA' no encontrado
```

```
## Error in checkFormulaData(formula, data, checkLHS = control$check.formula.LHS == : bad 'data': objeto 'USA' no encontrado
```

```
## Error in .stargazer.wrap(..., type = type, title = title, style = style, : objeto 'M1' no encontrado
```
<br /></center>

I next offer some quantities of interest to illustrate the effect that outgroup intolerance has on white Republican men in their attitudes toward democracy in these models. I take draws from a multivariate normal distribution of the model and isolate values for white, employed Republican men of average age and ideology. The outgroup intolerance measure and education variable are all that change in simulating these model outcomes.



