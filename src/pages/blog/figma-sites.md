---
id: "15"
layout: "../../layouts/BlogPostLayout.astro"
title: "Figma Sites"
description: "Vandaag heb ik me verdiept in Figma Sites, de nieuwe feature van Figma. Hoe goed is het? Of hoe slecht..."
date: "14 mei 2025"
speaker: "Front-End Focus"
image:
  url: "/assets/images/article_figma.png"
  alt: "Figma logo"
intro: "Vandaag heb ik me verdiept in Figma Sites, een nieuwe feature van Figma waarmee je als designer meteen websites kunt genereren vanuit je designs. Klinkt best handig, maar ik wilde weten hoe toegankelijk en semantisch de code daadwerkelijk is. Spoiler alert: niet best."
quotes:
  quote_one: "The true path to garbage code: Figma Sites"
  quote_two: "<div role='link'></div>"
content:
  paragraph_one: "Een div met een role link? Dat is iets wat wij er op de opleiding echt niet doorheen zouden krijgen. Toch kan Figma Sites dit blijkbaar wel. In het artikel wat ik heb gelezen laat Joe Dolson zien wat er allemaal mis is met de code die Figma Sites genereert. Denk aan meerdere elementen zonder logische semantiek, accessibility die compleet wordt genegeerd (!) en een totaal gebrek aan structuur. Dat is best wel schokkend, zeker als je bedenkt dat Figma Sites juist bedoeld is om het bouwen van websites toegankelijker te maken."
  paragraph_two: "Wat mij vooral opviel, is dat veel van de fouten die worden gemaakt eigenlijk heel makkelijk te voorkomen zijn — mits je je tool goed maakt. Een voorbeeld hiervan is het verkeerd gebruik maken van headings. In plaats van een hiërarchische structuur (h1 > h2 > h3), gebruikt Figma Sites vaak allemaal h1’s op één pagina, of helemaal geen headings. Voor screenreaders en SEO is dat echt NIET TE DOEN. Ook maakt het navigeren met toetsenbord bijna onmogelijk omdat de gegenereerde links geen echte links zijn, maar <div role='link'> elementen zonder ook maar focus states of keyboard interactie. Niet oké dus, zeker niet met de European Accessibility Act op de loer."
  paragraph_three: "Na het lezen van het artikel en het bekijken van voorbeelden, ben ik best teleurgesteld in deze tool van Figma. Ik snap dat het aantrekkelijk en leuk is om snel een klikbare website te genereren vanuit een design, maar dit mag in mijn optiek echt nooit ten koste gaan van toegankelijkheid of DUIDELIJKE webstandaarden. Voor nu denk ik: Figma Sites is leuk als prototype, maar als je een echte website wil maken? Dan toch maar gewoon handmatig bouwen.. Gelukkig kan ik dat."
---
