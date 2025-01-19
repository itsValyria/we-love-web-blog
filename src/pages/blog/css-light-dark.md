---
id: '7'
layout: '../../layouts/BlogPostLayout.astro'
title: 'CSS light-dark()'
description: 'Vandaag heb ik gelezen over de nieuwe CSS light-dark() functie die ik tegenkwam in de CSS Weekly.'
date: '16 januari 2025'
speaker: 'Mayank'
image:
  url: '/assets/images/article_light-dark.webp'
  alt: 'Illustration representing light and dark mode'
intro: 'Vandaag heb ik gelezen over de nieuwe CSS light-dark() functie die ik tegenkwam in de CSS Weekly nieuwsbrief. Ik vond dit interessant omdat ik zelf enkel een keer in het eerste jaar met een light/dark mode heb gewerkt, en ik het liefst binnenkort dit bij een privé project wil implementeren. light-dark() is dus een functie die het makkelijker maakt om websites te bouwen die de preferred color scheme van de user respecteren, terwijl je op het zelfde moment zonder veel extra code de mogelijkheid hebt het color scheme te overriden.'
quotes:
  quote_one: '"System colors have the ability to react to the current used color scheme value. The light-dark() function exposes the same capability to authors."'
  quote_two: '"A brief note about accessibility: When implementing a color system, be sure to pick color pairings that meet color contrast requirements."'
content:
  paragraph_one: 'Browsers hebben een ingebouwd "color-scheme" mechanisme, die je kan gebruiken met de color-scheme CSS property of de bijpassende meta tag. Je kunt color scheme op light of dark zetten, om te laten zien welke mode de pagina support. Je kan dus ook light en dark daar neerzetten, om aan te geven dat een pagina beide support. Normaal gezien zou je dit dan op het html element toepassen, waarbij je eigenlijk aan de browser aangeeft van: Hey browser, deze pagina support zowel dark en light mode, kijk even bij de user welke hij graag wilt!" De browser gebruikt dan het gekozen color scheme om dingen te bepalen als de background, text color, scrollbars, form elementen, etc. Het artikel gaf duidelijk aan dat color-scheme iets compleet ander concept is dan de prefers-color-scheme media query, en dat was inderdaad hetgeen wat ik in het eerste jaar heb gebruikt. De media query kijkt alleen daar de user preferences, en daarom is het een goed idee om als je de media query wilt gebruiken, ze ook te pairen, zodat scrollbars en form controls ook betere default styles krijgen. Interesting.'
  paragraph_two: 'Tot nu, was color-scheme eigenlijk een one way street. Browsers kunnen color-scheme gebruiken om de default en system colors aan te passen, maar programmeurs kunnen het niet in hun eigen code gebruiken om hun eigen custom styling toe te passen. Dat is waar de light-dark() functie van pas komt! Zo heb ik naar een aantal code snippets gekeken, in de eerste snippet kun je zien hoe alle links in light mode hotpink zijn, en alle links in dark mode deeppink. Het is een clean en straight forward manier om een style toe te passen, wat in het verleden meerdere CSS regels en media queries nodig zou hebben. Ook hoeven de twee kleuren niet hard coded te zijn, het kunnen ook custom properties zijn! light-dark() is sinds begin 2024 available, voor oudere browsers is het gebruik van LightningCSS of PostCSS een mogelijkheid.'
  paragraph_three: 'Het meeste is uit deze functie te halen door themed custom properties op te zetten. Daarbij hoort code snippet 2. Je kunt custom properties dus opzetten met light-dark, waardoor de hele pagia nu automatisch werkt met beide light en dark mode, zonder dingen aan te passen op component level. Het belangrijkste is dat light-dark gebonden is aan het kleurenschema, en niet aan de voorkeur van de gebruiker. Het respecteert de voorkeur van de gebruiker (zonder media query!) en kan ook worden overschreven, door bijvoorbeeld een thema toggle met een beetje JavaScript. Ook stond het in het artikel een voorbeeld dat hetzelfde stukje code, zonder light-dark(), wel vier keer een declaratie van de custom properties nodig had, waar dat met light-dark() maar één keer was. Vet!'
---
<br>

```css
:any-link {
  color: light-dark(DeepPink, HotPink);
}
```
<br>

```css
html {
  --accent: light-dark(DeepPink, HotPink);
  --bg: light-dark(White, Black);
  --fg: light-dark(Black, White);
}
```