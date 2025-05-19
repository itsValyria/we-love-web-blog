---
id: "13"
layout: "../../layouts/BlogPostLayout.astro"
title: "Browsers & HTML"
description: "Vandaag kwam Niels Leenheer een talk geven over Browsers en HTML, vooral over the old stuff!"
date: "25 april 2025"
speaker: "Niels Leenheer"
image:
  url: "/assets/images/article_niels.jpg"
  alt: "Old web browser"
intro: "Vandaag kwam Niels Leenheer langs bij ons op school voor een talk over browsers, HTML en vooral: resilience. Geen React, geen Svelte, geen moderne frameworks. Gewoon back to basics. En het bleek best interessant."
quotes:
  quote_one: "HTML is gemaakt voor mensen. Mensen maken fouten. Dus HTML vergeeft ze ook."
  quote_two: "Je kunt `<a<a<a<a>` typen en je browser snapt het nog steeds."
content:
  paragraph_one: "Niels werkt bij Salonhub, een bedrijf dat kassasystemen maakt voor kapsalons – grote kans dat je daar ooit iets van gebruikt hebt. Maar uiteindelijk is hij gewoon een web developer, net als wij. Zijn talk ging over hoe HTML ontworpen is om fouten op te kunnen vangen. Dat noem je resilience. Als je een fout maakt in JavaScript? Dan breekt alles. Maar in HTML? Dan werkt het meestal nog gewoon. En dat is geen bug, dat is juist een feature."
  paragraph_two: "Hij legde ons uit hoe dat komt: tussen je HTML document en wat je uiteindelijk op het scherm ziet (de DOM), zit een tokenizer en een tree builder. De tokenizer leest je HTML letter voor letter en probeert daar dan logica van te maken. En als het ergens een foutje tegenkomt? Dan stopt hij niet. Er zijn zelfs 68 verschillende states die die tokenizer kent. Daardoor kun je dingen typen als `<a<a<a<a>`, maar zal je zien dat de tokenizer gewoon door blijft gaan. Het klinkt gek, maar dit is precies waarom HTML zo robuust is. Het is ontworpen om te werken, ook als het niet perfect geschreven is."
  paragraph_three: "We kregen ook een mini-lesje in nostalgie (vooral voor de docenten): <blink> werkt niet meer, <marquee> nog wel (maar je moet het natuurlijk niet gebruiken). En <noscript>? Daarmee kun je content laten zien als JavaScript niet werkt. Maar verwacht er niet te veel van, want je kunt het niet stylen en geen script tag erin zetten... want uh.. no script. Uiteindelijk was dit een hele interessante talk over hoe browsers eigenlijk proberen ons te helpen, zelfs als we sloppy code schrijven. Het deed me even beseffen hoe krachtig HTML eigenlijk is."
---
