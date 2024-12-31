---
title: "TIVIA Satakunta ry:n uudet verkkosivut"
excerpt: "Tivia Satakunta on toteuttanut uudet verkkosivunsa käyttäen moderneja teknologioita. Sivut asuvat Cloudflaren serverless-ympäristössä (Pages, Workers), generoidaan ja päivitetään automaattisesti GitHub Actionsilla käyttäen Next.js -sovelluskehystä."
coverImage: "/assets/blog/default-cover.png"
date: "2024-12-31T08:05:26.047Z"
author:
  name: Heikki Lampen
  picture: "/assets/blog/authors/default-avatar.png"
ogImage:
  url: "/assets/blog/default-cover.png"
---

Tivia Satakunta ry on toteuttanut uudet verkkosivunsa käyttäen moderneja työkaluja.

Tavoitteena oli välttyä käyttöjärjestelmän ylläpidolta, tehdä blogien luominen kaikille helpoksi ja oppia uusia teknologioita.

Sivujen sisältöä hallitaan [GitHubissa](https://github.com/TIVIA-Satakunta/tiviasatakunta.fi). Blogit generoidaan Markdown-tiedostoista HTML-muotoon Next.js -sovelluskehyksellä, ja päivitetään Cloudflareen automaattisesti kun `main`-haaraa päivitetään git-repositoriossa.

Pohjaksi projektille valikoitui [OpenNext for Cloudflare](https://github.com/opennextjs/opennextjs-cloudflare) ja malliksi koodia [vercel-blog-starter](https://github.com/opennextjs/opennextjs-cloudflare/tree/main/examples/vercel-blog-starter) esimerkistä.

Tunnusten luomisen jälkeen projektiin kului muutamia päiviä, osan aikaa mennessä DNS-tietueiden muutosten päivitysten levitessä maailmalle. Negative TTL oli kohtalaisen pitkä oletuksena, joten uuden verkkotunnuksen kanssa hetki saada Cloudflare Pages käyttöön.

Muutamaa eri sovelluskehystä koitettua, valikoitui hyvien esimerkkien vuoksi OpenNextit Cloudflarelle optimoitu staattista sisältöä generoiva työkalu. Dynaamista sisältöä ei tässä vaiheessa vielä luotu.

Kirjastojen päivitysten jälkeen esimerkkikoodit tarvitsivat pieniä muutoksia toimiakseen, mutta kokonaisuutena sivujen tekeminen tuntui helpolta, vaikka aikaisempi web-kehityskokemus oli ainakin vuosikymmenen takaa.

Iso osa ajasta kului parin hassun kuvatiedoston tekemisen kanssa, koska graafista osaamista löytyi web-kehitysosaamistakin vähemmän. Käyttäjät voivat halutessaan lisätä oman avatar-kuvansa ja blogikohtaisen kansikuvan, tai käyttää näitä oletuskuvia.

Tällä pääsimme alkuun ja aika näyttää minkälaista sisältöä sivuille jatkossa luodaan.

Mukavaa uutta vuotta 2025 lukijoille!
