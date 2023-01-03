# GitHub Pages

Diese Seite wurde mit GitHub Pages erstellt, eine sehr einfache und coole Art, statischen Content als Webseite zur Verfügung zu stellen.
GitHub Pages werden als Markdown geschrieben und mit Hilfe des static site generators jekyll gebaut.

* Editor: Visual Studio Editor
  * [Plugins](vs-code-plugins.md)
* Markdown Engine: Kramdown
* Theme: [slate](#github-pages-theme-slate) via jekyll-remote-theme (Plugin)

**Warum habe ich mich gerade für GitHub Pages entschieden?**

Dass ich meine Erfahrungen und Kenntnisse für mich dokumentieren und anderen zur Verfügung stellen will, hatte ich von Beginn an vor. Allerdings dachte ich eher an eine private Doku, irgendetwas gewöhnliches wie Office (Writer, Calc, ...) oder Notepad++.
Als ich mich dann dafür entschieden habe, meine Dokumentation öffentlich zu machen, überlegte ich, wie ich es am besten anstelle. Auf meinem Server ein WordPress bereitzustellen, war mir zu aufwändig, denn ich wollte sofort losdokumentieren. Außerdem müsste ich Plugins und Themes installieren, konfigurieren und das WordPress regelmäßig patchen und Backup einrichten. Wie gesagt: zu aufwändig. Eine kostenlose WordPress Instanz (managed) wollte ich auch nicht, denn ich will keine Werbung in meiner Doku haben und Geld für's Hosting ausgeben will ich auch nicht. So hat mich **[Christopher](https://github.com/beechesII)** auf die coole Idee mit den GitHub oder GitLab Pages gebracht und ich habe mir das mal genauer angesehen. GitLab nutze ich auf Arbeit schon so viel - deswegen habe ich mich für GitHub entschieden.

## GitHub Pages Custom Domain

Da ich mir die Url der Page nicht merken konnte, hielt ich es für sinnvoll, sie unter einer custom domain verfügbar zu machen:

1. (Sub-)Domain ausdenken und CNAME auf die GitHub-User-Domain setzen (hier: balkonkraftwerk.gessnet.de -> hegessne.github.io)
2. DNS Eintrag prüfen

```bash
root@linux01:~# dig CNAME balkonkraftwerk.gessnet.de

; <<>> DiG 9.16.33-Debian <<>> CNAME balkonkraftwerk.gessnet.de
;; global options: +cmd
;; Got answer:
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 50867
;; flags: qr rd ra; QUERY: 1, ANSWER: 1, AUTHORITY: 0, ADDITIONAL: 1

;; OPT PSEUDOSECTION:
; EDNS: version: 0, flags:; udp: 512
;; QUESTION SECTION:
;balkonkraftwerk.gessnet.de.	IN	CNAME

;; ANSWER SECTION:
balkonkraftwerk.gessnet.de. 600	IN	CNAME	hegessne.github.io.

;; Query time: 69 msec
;; SERVER: 172.17.5.1#53(172.17.5.1)
;; WHEN: Mon Nov 21 15:23:02 CET 2022
;; MSG SIZE  rcvd: 87
```

3. in Repo Settings -> Pages -> Custom Domain -> Domain eintragen
4. SAVE
5. Anschließend wird die Seite mit den geänderten Properties neu gebaut und deployt (kann man in Actions bestaunen)

weitere Infos weiter unten in den Links

6. Haken setzen bei ENFORCE HTTPS
7. Warten und freuen, dass die Seite über die Custom Domain und per HTTPS erreichbar ist

## GitHub Pages Theme slate

* [Theme Slate bei GitHub](https://github.com/pages-themes/slate)

## GitHub Pages - meine Meinung - Pros und Cons

### Cons

* Bilder einfügen und skalieren ist etwas umständlich
* Vorschau im Editor (VSCode) nicht immer zuverlässig - das endgültige Ergebnis sieht man erst nach dem Rendering/ Deployment

### Pros

* Vorteile des Arbeitens im Git: Branches, Releases (Tags)
* VSCode Plugins unterstützen das Arbeiten

### Fazit

Die Erstellung der Doku mit GitHub Pages ist eine coole Sache. Arbeiten mit Git und CI/CD-Pipelines gehören zu meinem Arbeitsalltag und sind von Vorteil. Im Gegensatz zu einem WordPress Blog hat es auch einen nerdigen Charme. Auch das Arbeiten im VSCode macht natürlich sehr viel Spaß, aber die [Cons](#cons) zeigen auch, dass es die eine oder andere Herausforderung zu bewältigen gibt. Eine interessante Erfahrung ist es auf jeden Fall und ich habe auch wieder etwas neues gelernt. ;-)

## GitHub Pages Blog - How to

will ich noch machen...

## Links

Hier einige nützliche Links, wenn man sich der Thematik nähern will:

### GitHub Pages Dokumentation

* [GitHub Pages](https://docs.github.com/en/pages)
* [About GitHub Pages and Jekyll](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/about-github-pages-and-jekyll)
* [Quickstart for writing on GitHub](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/quickstart-for-writing-on-github)
* [GitHub Pages Custom Domain](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site)

### GitHub Pages Blog

* [Creating a blog using GitHub Pages - David's Blog](https://dfederm.com/creating-a-blog-using-github-pages/)

### Markdown

* [MarkdownGuide - Getting Started](https://www.markdownguide.org/getting-started/)
* [MarkdownGuide - Hacks](https://www.markdownguide.org/hacks/)
* [MarkdownGuide - Cheat Sheet](https://www.markdownguide.org/cheat-sheet)
* [Markdown Cheat Sheet](https://www.freecodecamp.org/news/markdown-cheat-sheet/)
* [Markdown Linting Rules](https://github.com/DavidAnson/markdownlint/blob/main/doc/Rules.md)
* [W3schools.io - Markdown Tutorial](https://www.w3schools.io/file/markdown-introduction/)

### Kramdown

* [Kramdown Dokuseite](https://kramdown.gettalong.org/)
* [GitLab - Kramdown Tipps und Tricks](https://about.gitlab.com/blog/2016/07/19/markdown-kramdown-tips-and-tricks/)
