---
layout: post
title: GitHub Codespaces aneb VS Code na VPS
subtitle: Dopřejte si trochu luxusu
categories: vychytávky
tags: github vps
sidebar: []
---

Nedávno mi přišel e-mail, že jsem byl přidán do beta testování funkce Codespaces na GitHubu. Stručně, Codespaces má být systém ve kterém si vytvoříte vlastní prostředí pro váš repozitář, do kterého si nainstalujete všechny potřebné knihovny, SDK a balíky. Server, na kterém to všechno běží, si platíte u GitHubu a můžete na něj kdekoliv a kdykoliv přejít přes web do webové, narozdíl od výchozího webového VS Code plně vybavené, verzi VS Code nebo nainstalovaný VS Code a upravovat nebo testovat kód.

Hodí se pro lidi, kteří nechtějí tahat např. do školy nebo do práce, kde nesmí instalovat externí aplikace, svůj vlastní notebook.
Parametry

V betě je možné testovat pouze výchozí možnost 4 jádra + 8GB RAM + 32GB úložiště, což definitivně stačí pro osobní a malé projekty. Do konce bety neplatíte nic, ale 4 jádra vyjdou na $0.36 (asi 8,3 kč) za hodinu, tj za hodinu aktivního používání. Codespace se vám automaticky vypne, pokud není po stanovenou dobu nepoužíván, takže můžete předejít placení katastrofických částek.
![Ceny Codespaces](/assets/images/codespaces/1.jpg)

Je to určitě výhodnější, než si platit např. hotové VPS, pokud ho tedy nepoužíváte i na něco smysluplnějšího.
Moje zkušenost

Samozřejmě jsem nemohl odolat a na OpenCanteen jsem si jeden nechal vytvořit, aniž bych věděl do čeho se vrhám.

Codespace se vytváří jednoduše kliknutím na tlačítko "Code" ve vašem repozitáří, kde se vám nově zobrazí možnost si Codespace vytvořit.

Ve výchozím stavu běží server na Ubuntu. Pokud nenajdete docker obraz nebo devcontainer konfigurační soubor, musíte si samozřejmě vše nainstalovat sami, což zas tolik nevadí, protože to nejspíš budete dělat jen jednou, pokud si nebudete s obrazem stroje nějak zahrávat.

Instalace všeho však probíhá svižně, jelikož asi v Microsoftu mají na rychlejší internet, než já. Samozřejmě vše musíte instalovat skrze terminál (což mě celkem ranilo, jelikož instalovat Android SDK pro flutter byla celkem fuška).

Pokud používáte Settings Sync ve VS Code, automaticky se vám synchronizují nastavení a rozšíření. Pro pokročilé upravení prostředí slouží konfigurační soubor devcontainer.json
![Ceny Codespaces](/assets/images/codespaces/2.jpg)

Jakmile máte všechno nastavené, už stačí jen využít starého známého Visual Studio Code, které funguje úplně stejně jako na lokálním zařízení. Na Codespace se můžete kdykoli připojit přes webovou adresu.

Za mě velice praktické pro dříve uvedené typy lidí, už jen záleží, jestli se to zrovna vám za ty peníze vyplatí. Dokumentace je možná trochu chaotická, alespoň pro uživatele co se nevyznají v technologiích jako kontejnery či docker a většiny funkcí využije jen skutečný poweruser (což já určitě nejsem).