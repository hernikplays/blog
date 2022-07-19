---
layout: post
title: Automatizace, automatizace, automatizace
subtitle: Ulehčujeme si život
categories: programování
tags: automatizace technologie
sidebar: []
---

Roboti nám brzo vezmou práci, ale mně to (prozatím) nevadí. Já nechávám robůtky pracovat za mě a ulehčovat mi práci. A vy byste měli taky! Pokud teda programujete, jinak nevím.

Nedávno jsem objevil krásy zvané GitHub Actions a musím říct, že je to opravdu radost. Nikdy předtím jsem nedokázal pochopit jejich praktičnost, než jsem pracoval na [OpenCanteen](https://github.com/hernikplays/opencanteen). Sestavovat, podepisovat a nahrávat mě opravdu nebavilo a ještě s mým pomalým PC v kombinaci s pomalým internetem to nešlo zrovna rychle. Pak jsem si vzpomněl na GitHub Actions. Místo toho, abych dělal cokoliv produktivního, jsem strávil celé odpoledne nastavováním Actions, aby mi při novém tagu automaticky sestavil a publikoval vydání aplikace do Google Play.

Ta první část šla skvěle, avšak nahrávání do Google Play bylo o něco složitější, dokud jsem neobjevil hotové a, prozatím bezplatné, řešení [CodeMagic](https://codemagic.io/start/). 

Jednoduše jsem napojil repozitář, nastavil podepisovací a nahrávací údaje a všechno hned jelo! Byla to radost pro někoho tak líného jako jsem já. I přesto, že jsem sám reálně nic neudělal, cítil jsem, že jsem dosáhl něčeho úžasného.

A určitě to lze dotáhnout ještě dál, už teď používám Actions pro automatickou analýzu kódu, a kdybych si vytvořil testy tak by mi to určitě i otestovalo celou aplikaci.

Pak jsem si řekl, že by možná mohl někdo chtít do mé aplikace přispět svým kódem. Protože chci v tom mít pořádek, hned jsem začal projíždět GitHub Marketplace pro nějaké akce na pull requesty. Hned jsem jich několik objevil.

Velice jsem ocenil akci, která mi automaticky přidala labely podle souboru, který byl v PR upraven.

Určitě nepotřebujete nutně automatizovat všechno, pokud máte např. soukromý či malý projekt. Nicméně si to můžete aspoň otestovat a případně využít v budoucnu tak se do toho pusťte! Automatizovat můžete všechno možné. Určitě budete mít dobrý pocit, když se vaše akce spustí a úspěšně se dokončí.
