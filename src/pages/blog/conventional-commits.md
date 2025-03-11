---
id: "10"
layout: "../../layouts/BlogPostLayout.astro"
title: "Convent. Commits"
description: "Vandaag heb ik mezelf op eigen initiatief verdiept in Conventional Commits."
date: "28 februari 2025"
speaker: "their website!"
image:
  url: "/assets/images/conventional-commits.jpeg"
  alt: "Conventional commits"
intro: "Vandaag heb ik mezelf op eigen initiatief verdiept in conventional commits. Dit heb ik gedaan omdat dit bij Triple gebruikt wordt, en omdat ik nog nooit eerder heb gewerkt met een specifieke structuur voor commits in mijn eigen projecten of zelfs school projecten. Daar wilde ik graag verandering in brengen."
quotes:
  quote_one: '"Ik wilde er graag meer over leren omdat ik nog nooit met een conventie heb gewerkt voor commits."'
  quote_two: '"Een manier van commits schrijven als deze voelt erg overzichtelijk."'
content:
  paragraph_one: "Eerst heb ik me verdiept in wat conventional commits nou echt is. Het antwoord hierop is dat conventional commits eigenlijk een soort conventie is voor commit messages. Er zijn een aantal simpele regels, die niet alleen commits overzichtelijk maken, maar ook ervoor zorgen dat het makkelijker wordt om automated tests te schrijven op basis van de commits. Hoe dat precies werkt, stond niet uitgelegd en was op dit moment ook niet mijn focus."
  paragraph_two: "Hierna heb ik gekeken in hoe de structuur van zo'n commit er nou eigenlijk uit ziet. Het komt er op neer dat je eigenlijk allemaal verschillende types hebt, zoals bugfix, chore, en feature. Door deze types te gebruiken kun je gelijk een beetje een idee krijgen van wat de inhoud van de commit is, zonder de message te lezen. Ook kun je een breaking change toevoegen, wat aangeeft dat er een grote verandering is geweest, bijvoorbeeld iets met de API die je gebruikt."
  paragraph_three: "Nadat ik me verdiept heb in hoe zo'n commit er uit ziet, ben ik gaan kijken hoe het op mijn stage word toegepast. Omdat deze blog openbaar is, ga ik dat hier niet delen, maar ik heb het wel ingeleverd als bewijslast voor school. Ik ben het wel in mijn eigen stage project gaan gebruiken, en ook in een van mijn privé projecten ben ik ermee begonnen! Ik denk niet meer dat ik snel terug wil, want het ziet er netjes uit en het is erg overzichtelijk! Onderaan zie je nog wat voorbeeldjes. Meer info kun je bekijken op hun website, conventionalcommits.org!"
---

```
// Voorbeeld van de template

<type>[optional scope]: <description>`

[optional body]

[optional footer]

// Voorbeeld van mijn commits na conventional commits

--> Stage
chore(pokeapp): added active states to the side menu
fix(pokeapp): added inline styles for older devices

--> Privé
chore(fixes #1): Setup project with Astro
```
