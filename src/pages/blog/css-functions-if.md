---
id: "12"
layout: "../../layouts/BlogPostLayout.astro"
title: "CSS Functions"
description: "Vandaag heb ik me verdiept in het artiekl over CSS Functions en CSS if() uit de CSS Weekly!"
date: "12 maart 2025"
speaker: "CSS Weekly"
image:
  url: "/assets/images/css.png"
  alt: "CSS Logo"
intro: "Vandaag heb ik me verdiept in het artikel uit de CSS Weekly ocer CSS function en CSS if(), geschreven door Bramus. Eerder heb ik me al verdiept in de CSS light-dark() functie, maar sinds de nieuwe Chrome Canary update zijn ook nested container queries support én CSS if() is toegevoegd! En als ik Bramus mag geloven, is het een game changer."
quotes:
  quote_one: '"It is a game changer!"'
  quote_two: '""'
content:
  paragraph_one: "Wat wel jammer is, is dat deze post tot nog toe gaat over een upcoming feature: het is op dit moment toegevoegd aan Chrome Canary als je de experimental web features flag enabled hebt. Het is dus nog niet beschikbaar in de reguliere versie van Chrome. Wat Bramus gebouwd heeft, is een custom light-dark() die values returned op basis van welk theme geactiveerd is. Dat betekent dat, unlike de normale light-dark() deze custom versie niet gelimiteerd is aan een kleur value, maar dit kan met élke value. Een nadeel, deze custom versie kan niet responden op de local color-scheme, enkel op de light-dark media preference... tot nu. Deze limitatie kon weggehaald worden met support voor nested media queries en/of CSS if(), en beide zijn nu toegevoegd!"
  paragraph_two: "Het prototype wat Bramus gebouwd heeft, beschikt over een CSS Function die 2 arguments heeft, een --light en --dark. Met een container query kun je luisteren naar de container style, en daarmee kun je de --scheme (de kleur die je wisselt bijvoorbeeld) overschrijven naar --dark. Dus overal waar jij --scheme hebt staan, verschijnt dan de dark kleur in plaats van light. VET!"
  paragraph_three: "Maar, as of Chrome Canary 135 is de inline if() ook available in CSS, en dankzij deze functie kun je het extra container element wat de container query approach nodig heeft weg laten, omdat je met conditions een value kan selecteren direct in de declaration. Deze manier heeft dus een heleboel minder code. Interesting. Ook heeft Bramus om het af te sluiten nog even een Galaxy brain meme toegevoegd om te laten zien hoe excited hij is, hahaha. "
---

```css
/* Custom light dark using container query */
@function --light-dark(--light, --dark) {
  /* Default to the --light value */
  result: var(--light);

  /* If the container is set to "dark", use the --dark value */
  @container style(--scheme: dark) {
    result: var(--dark);
  }
}
```

```css
/* Custom light dark using inline if() */
@function --light-dark(--light, --dark) {
  /* If style is set to dark, --scheme is --dark */
  result: if(
    style(--scheme: dark): var(--dark) ; /* Else, use the --light value */ else:
      var(--light)
  );
}
```
