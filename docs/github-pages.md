# GitHub Pages

GitHub Pages werden als Markdown geschrieben und mit Hilfe des static site generators jekyll gebaut.

* Editor: Visual Studio Editor
  * [Plugins](vs-code-plugins.md)
* Markdown Engine: Kramdown
* Theme: architect via jekyll-remote-theme (Plugin)

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

## Links

Hier einige nützliche Links, wenn man sich der Thematik nähern will:

### GitHub Pages Dokumentation

* [GitHub Pages](https://docs.github.com/en/pages)
* [About GitHub Pages and Jekyll](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/about-github-pages-and-jekyll)
* [Quickstart for writing on GitHub](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/quickstart-for-writing-on-github)
* [GitHub Pages Custom Domain](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site)

### Markdown

* [MarkdownGuide - Getting Started](https://www.markdownguide.org/getting-started/)
* [MarkdownGuide - Hacks](https://www.markdownguide.org/hacks/)
* [MarkdownGuide - Cheat Sheet](https://www.markdownguide.org/cheat-sheet)
* [Markdown Cheat Sheet](https://www.freecodecamp.org/news/markdown-cheat-sheet/)
* [Markdown Linting Rules](https://github.com/DavidAnson/markdownlint/blob/main/doc/Rules.md)

### Kramdown

* [Kramdown Dokuseite](https://kramdown.gettalong.org/)
* [GitLab - Kramdown Tipps und Tricks](https://about.gitlab.com/blog/2016/07/19/markdown-kramdown-tips-and-tricks/)
