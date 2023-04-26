# Doku zum Aufbau und Betrieb meines Photovoltaik Balkonkraftwerkes

Diese Seite dokumentiert den Aufbau und Betrieb meiner Mini PV-Anlage (Balkonkraftwerk).
Sie soll mein Wissen und meine Erfahrung dokumentieren, zum selbst ausprobieren anregen und meinen Fortschritt in einem Blog veranschaulichen.
Außerdem ist das meine erste Seite mit GitHub Pages - dazu weiter unten mehr in [GitHub Pages](github-pages.md)

---

Inhalt

- [Doku zum Aufbau und Betrieb meines Photovoltaik Balkonkraftwerkes](#doku-zum-aufbau-und-betrieb-meines-photovoltaik-balkonkraftwerkes)
  - [Einleitung und Motivation](#einleitung-und-motivation)
    - [1. Teilnehmen an Energiewende](#1-teilnehmen-an-energiewende)
    - [2. Erfahrung sammeln und Wissen teilen](#2-erfahrung-sammeln-und-wissen-teilen)
    - [3. Wirtschaftlichkeit](#3-wirtschaftlichkeit)
    - [4. Nachhaltigkeit](#4-nachhaltigkeit)
  - [Podcast-Links](#podcast-links)
  - [Selberbauen oder Fertiglösung?](#selberbauen-oder-fertiglösung)
  - [Auf gehts - wir fangen mal an](#auf-gehts---wir-fangen-mal-an)
    - [1. Einzel-Komponenten](#1-einzel-komponenten)
    - [2. Montage der PV Module](#2-montage-der-pv-module)
    - [3. Auflagen und Anmeldungen](#3-auflagen-und-anmeldungen)
  - [Links Informationen Photovoltaik/ Solar-Anlagen allgemein](#links-informationen-photovoltaik-solar-anlagen-allgemein)
  - [Links Informationen Balkonkraftwerke](#links-informationen-balkonkraftwerke)
  - [GitHub Pages](#github-pages)

---

## Einleitung und Motivation

Das erste Mal bin ich beim Hören des Podcasts (siehe unten) auf der langen Urlaubsfahrt mit Balkonkraftwerken in Berührung gekommen und ich fand das Thema sofort interessant. Es gibt kaum Hindernisse - es kann praktisch jeder machen. Egal ob Mietwohnung, Gartengrundstück oder Eigenheim - eine kleine PV-Anlage mit bis zu 600 Watt Ausgangsleistung darf jeder zu Hause betreiben, ohne dass sie ein Elektriker oder der Netzanbieter abnehmen lassen muss.

**Allerdings sollte man es nicht mit einer Notstromversorgung verwechseln, denn wenn keine Netzspannung anliegt, schaltet sich der Wechselrichter aus Sicherheitsgründen automatisch ab.**

**Die folgenden Rahmenbedingungen stehen dabei im Vordergrund:**

- maximale Einspeiseleistung von 600 Watt (VDE-konform ohne Elektriker und ohne Abnahme)
- keine Einspeise-Vergütung (EEG-Umlage), nur private Verwendung
- keine Stromspeicherung
- Voraussetzungen müssen erfüllt sein
  - moderner Stromzähler (mit Rücklaufsperre)
  - Stromleitungen müssen stark genug sein (am besten nicht älter als 40 Jahre alt)
- Anmeldung bei der Bundesnetzagentur (Marktstammdatenregister) und beim Netzanbieter

Für mich steht nicht die Wirtschaftlichkeit der Anlage im Vordergrund - meine Motivation erstreckt sich in folgenden Punkten:

### 1. Teilnehmen an Energiewende

Ich möchte gern meinen Beitrag an der Energiewende und einer dezentralen Stromversorgung leisten. Für mich ist es damit nicht vordergründig, dass sich die PV-Anlage nach x Jahren amortisiert. Jede Kilowattstunde, die durch mein Balkonkraftwerk produziert wird, reduziert den CO2-Ausstoß, weil dafür keine Verbrennung fossiler Energieträger wie Gas, Öl oder Kohle notwendig ist.
Außerdem sind die PV-Module am Haus sichtbar und vielleicht beschäftigt sich dadurch der eine oder andere in meiner Nachbarschaft mit dem Thema oder schafft sich sogar selbst ein Balkonkraftwerk an.

### 2. Erfahrung sammeln und Wissen teilen

Diesen Punkt hatte ich erst an dritter Stelle und ohne "Wissen teilen" geschrieben, aber durch die Wissensteilung ist dies für mich nochmal umso wichtiger gewesen. Außerdem wurde ich mehrmals gefragt, ob ich meine Erfahrungen dokumentieren könne (**Danke [Andreas](https://github.com/avalor1)!**) - das war soewieso mein Anspruch, nur nicht öffentlich.
Erneuerbare Energien bzw. wie in diesem Fall die Photovoltaik interessieren mich sehr und ich habe mich dafür entschieden, mir mein Balkonkraftwerk selbst zusammenzubauen.
Voraussetzung dafür ist das notwendige Know-How, deshalb lagen zwischen dem Hören des ersten Podcasts dazu und der Bestellung des Inverters (=Gleichrichter) bei mir knapp 3 Monate.
Angefangen bei den rechtlichen Rahmenbedingungen, der Auswahl des Gleichrichters sowie der PV-Module, den Stromanschlüssen bis hin zur Standortwahl will alles gut recherchiert sein. Das war sehr interessant, hat aber auch viel Zeit gekostet und ich fühle mich in dieser Thematik nun viel sicherer.
Dieses Wissen möchte ich gern dokumentieren, falls ich es selbst nochmal nachlesen will, aber auch gern mit anderen teilen. Auch meine Erfahrungen werde ich aufschreiben, denn nicht alles ist mir immer gleich beim ersten Mal geglückt.
Vielleicht habe ich auch später einmal die Ambition, mir eine größere PV-Anlage aufs Dach zu bauen - da werden mir diese Erfahrungen sicher weiterhelfen. Ich möchte ja auch nicht zum Elektriker gehen und sagen: "Hier hast Du 15.000 Euro - bitte baue mir mal was aufs Dach." Da bin ich zu sehr Nerd, als dass ich genau wissen möchte, welche PV-Module in welcher Anzahl da verbaut werden usw...

### 3. Wirtschaftlichkeit

Natürlich ist die Verhältnismäßigkeit zwischen Investition und Nutzen nicht völlig egal. Ich sehe die Anschaffungskosten als eine Investition in die ersten beiden Punkte meiner Motivation und wenn sich die PV-Anlage auch wirtschaftlich lohnt, freut es mich natürlich umso mehr. Bei der Entwicklung der Energiepreise ist das wohl schon eher der Fall als man denkt... ;-)

### 4. Nachhaltigkeit

Beim Thema Energiewende und Umweltschutz geht es meiner Meinung nach auch um Nachhaltigkeit. Ich habe den Anspruch, so viel wie möglich regional zu kaufen. Zum Beispiel werde ich mir Stecker und Stromkabel im Baumarkt um die Ecke kaufen - auch wenn es bequemer wäre, dies in der Mittagspause im Internet zu bestellen. Auch den Stahl die die PV Modul Aufständerung werde ich lokal kaufen usw...
Natürlich ist der Anspruch z. B. für Wechselrichter und PV Module nur bedingt oder gar nicht umsetzbar, aber dennoch kann man einen Beitrag zur Nachhaltigkeit durch regionales Kaufen oder das Vermeiden von Versand-Lieferungen leisten.

## Podcast-Links

Besonders der erste Podcast hat mich erwischt - ich habe ihn auf der Urlaubsfahrt gehört und es hat mich sofort gepackt. So einfach? Das will ich auch.

- [Balkonkraftwerke und selbstgemachter Strom - c’t uplink 43.8](https://www.heise.de/news/Balkonkraftwerke-und-selbstgemachter-Strom-c-t-uplink-43-8-7126423.html)

weitere Podcasts zum Thema Balkonkraftwerk, die ich mir angehört habe und interessant waren

- [TechnikDiskutiert - Wie baue ich mir ein Balkonkraftwerk?](https://podcasts.google.com/feed/aHR0cHM6Ly9hbmNob3IuZm0vcy85MDhkYTEwNC9wb2RjYXN0L3Jzcw/episode/YWZhNmRlZDYtYzBiOC00ZTY3LTk1MDktN2E4ZDkxNjY5MDdk?sa=X&ved=0CAIQuIEEahcKEwjw0oChgbX7AhUAAAAAHQAAAAAQQw)

## Selberbauen oder Fertiglösung?

Wie oben bereits geschrieben, habe ich mich entschieden, eine PV-Anlage (Balkonkraftwerk) selbst zu bauen.
Diese Seite soll auch dazu dienen, relevante Details und Überlegungen zu dokumentieren, so dass die Hürde, es ebenfalls selbst zu bauen, gesenkt wird.
Fertiglösungen sind sicher auch OK, und ich denke, dass jede Anlage ein Schritt in die richtige Richtung zur dezentralen Energiegewinnung ist.

## Auf gehts - wir fangen mal an

### 1. Einzel-Komponenten

- [Wechselrichter/ Inverter](inverter.md)

- [PV Module](pv-module.md)

- [Verkabelung](stuff.md)

### 2. Montage der PV Module

- [Ausrichtung der PV Module](pv-module_ausrichtung.md)

- [Neigungswinkel der PV Module](pv-module_neigungswinkel.md)

- [Montage der PV Module - Dach, Schuppen, Balkon oder Fassade](pv-module_montage.md)

  - [Montage der PV Module auf Flachdach](pv-module_montage_dach.md)

  - [Bau der PV-Platten Halterung aus Winkelstahl (Eigenbau)](pv-module_montage_halterung_winkelstahl.md)

### [3. Auflagen und Anmeldungen](behoerdenkram.md)

## Links Informationen Photovoltaik/ Solar-Anlagen allgemein

- [Photovoltaik.org](https://www.photovoltaik.org/)
- [Photovoltaikforum](https://www.photovoltaikforum.com/)
- [Solaranlagen-Portal](https://www.solaranlagen-portal.com)

## Links Informationen Balkonkraftwerke

- [wohnglueck.de - Balkonkraftwerk: Lohnt sich eine Solaranlage für den Balkon?](https://wohnglueck.de/artikel/balkonkraftwerk-vorteile-nachteile-kosten-27810)
- [verivox.de - Balkonkraftwerk](https://www.verivox.de/photovoltaik/themen/balkonkraftwerk/)
- [homeandsmart.de - Balkonkraftwerk Test-Überblick 2022: Vorteile, Kosten & Modelle](https://www.homeandsmart.de/balkonkraftwerk-solaranlage-vergleich)
- [sonnstrom.de - Balkonkraftwerk](https://www.sonnstrom.de/Balkonkraftwerk.html)
- [computerbild.de - Balkonkraftwerke im Vergleich](https://www.computerbild.de/artikel/Balkonkraftwerk-Vergleichstabelle-32639441.html)
- [Anker.de -  Welche Vorteile haben Balkonkraftwerke und für wen sind sie geeignet?](https://de.anker.com/blogs/content/solarmodule-fuer-eigenbedarf-vorteile)

## [GitHub Pages](github-pages.md)
