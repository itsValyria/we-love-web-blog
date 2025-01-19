---
id: '7'
layout: '../../layouts/BlogPostLayout.astro'
title: 'CSS Wrapped 2024'
description: 'Vandaag heb ik de CSS wrapped doorgenomen die ik zag in de nieuwsbrief van Frontend Focus.'
date: '13 december 2024'
speaker: 'Google Chrome'
image:
  url: '/assets/images/article_css-wrapped.webp'
  alt: 'Illustration of the letters CSS'
intro: 'Vandaag heb ik de CSS wrapped doorgenomen die ik zag in de nieuwsbrief van Frontend Focus. Deze is uitgebracht door Google. In totaal highlight het Chrome DevRel team 17 nieuwe features die gereleased zijn in 2024. 5 components, 4 interacties en 8 DX features. Ik ben benieuwd of ik er een aantal ken, en of ik dingen kan gaan gebruiken in mijn projecten!'
quotes:
  quote_one: '"Chrome and CSS in 2024 journeyed through the forest, over the mountains, and across the seas…"'
  quote_two: '"2024 has been another amazing year for CSS!"'
content:
  paragraph_one: 'Components: over the mountains! De eerste is field-sizing. Zonder field-sizing moest je JavaScript gebruiken om karakters bij te houden en de element height or width groter te maken als de user meer text invoert. Nu is het een CSS one-liner. Interessant voor forms, al denk ik dat ik het niet snel zou gebruiken in een klassiek form, omdat ik het persoonlijk mooier vind als alle inputs een gelijke width hebben. Misschien voor de height kan het wel. Een andere interessante is exclusive <details>! Een common UI practice is een accordion component, die bestaat uit meerdere widgets die los van elkaar uitgeklapt kunnen worden, maar dus wel aan elkaar vast zitten. Dit is nu mogelijk met een paar detail elementen, door ze een name attribute te geven. Als je een andere detail tag opent van een groep, zal degene die je daarvoor geopend hebt automatisch dicht gaan. Dit is super handig voor FAQ paginas om de vragen te groeperen en de pagina overzichtelijk te houden. Ook een interessante: styleable <details>! Hier stond echt een supervette codepen bij. Je zou hiermee dus een accordion kunnen maken met een flex layout in de vorm van een row. Zo kun je een vettere variatie maken op een foto carousel.'
  paragraph_two: 'Interactions: Through the forest! De eerste is, custom scrollbars! Dit was al langer mogelijk, met webkit scrollbar, echter is er nu scrollbar-width en scrollbar-color! Dit geeft veel meer leuke opties. Ook kwam dit jaar natuurlijk de (cross document) view transitions! Dit hebben wij al gebruikt in onze projecten en ook in onze codespikes, dus ik ga daar niet te veel woorden aan vuil maken. Echter is het heel leuk om deze terug te zien in de CSS Wrapped. En dan de laatste, nog eentje die ik ken, namelijk scroll driven animations! Ook deze kwam terug in onze code spikes in sprint 17.'
  paragraph_three: 'Developer Experience: across the seas! Als eerst, backdrop inheritance. Voorheen haalde het backdrop psuedo element nergens een kleur vandaan, geen inherit. Vanaf Chrome 122, is het ::backdrop psuedo element omgezet tot een tree abiding element, wat betekent dat hij zijn kleur inherit van het originating element. Ook is light-dark() nieuw! (Edit januari 2025: hier heb ik een compleet artikel over gelezen hihi!) De light-dark functie staat developers toe om light en dark modes te customizen. Next, de Popover API. Hiermee kun je layered interfaces maken zoals tooltips, menu etc. Het enige wat je nodig hebt is een button om de popover te triggeren, en een element dat de popover is.'
---