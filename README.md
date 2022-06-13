# wilkerstrasse.ch

Website für das Strassenfest an der Wilkerstrasse

## HowTo

- Repository machen und in den 'Settings' einstellen, dass [GitHub Pages](https://pages.github.com) eine Webseite davon serviert.
- Bei [cyon.ch](https://www.cyon.ch/domains/) eine Domain kaufen.
- [CNAME](CNAME) in GitHub auf die neu gekaufte Domain umbiegen.
- Bei Cyon CNAME und [A-Record](https://docs.github.com/en/free-pro-team@latest/github/working-with-github-pages/managing-a-custom-domain-for-your-github-pages-site#configuring-an-apex-domain) für GitHub Pages einstellen.
- Adventskalender-Webseite in einen eigenem [branch](https://git-scm.com/docs/git-branch) parkieren (siehe alle Branches hier: https://github.com/habi/wilkerstrasse.ch/settings/branches) und einen Sommerfest-Branch machen.
- [Sommerfest-Branch](https://github.com/habi/wilkerstrasse.ch/tree/strassenfest) editieren und wieder in den `main`-Branch `merge`n, damit dieser Code auf wilkerstrasse.ch auftaucht.