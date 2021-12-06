# wilkerstrasse.ch

Website für den Adventskalender an der Wilkerstrasse

## HowTo

- Repository machen und in den 'Settings' einstellen, dass [GitHub Pages](https://pages.github.com) eine Webseite davon serviert.
- Bei [cyon.ch](https://www.cyon.ch/domains/) eine Domain kaufen.
- [CNAME](CNAME) in GitHub auf die neu gekaufte Domain umbiegen.
- Bei Cyon CNAME und [A-Record](https://docs.github.com/en/free-pro-team@latest/github/working-with-github-pages/managing-a-custom-domain-for-your-github-pages-site#configuring-an-apex-domain) für GitHub Pages einstellen.
- Tabelle von Andrea mit den Adventsfenstern auf [GeoJSON.io](http://geojson.io) händisch in eine [GeoJSON-Datei](https://git.io/JkdqT) umklicken.
- Diese GeoJSON-Datei in einer [uMap](https://wiki.openstreetmap.org/wiki/DE:UMap) als Datenquelle einfügen (dafür bei der [Datei hier im GitHub Repository](https://github.com/habi/wilkerstrasse.ch/blob/main/adventsfenster.geojson) oben rechts auf 'Raw' klicken und [diese URL](https://raw.githubusercontent.com/habi/wilkerstrasse.ch/main/adventsfenster.geojson) als 'Remote Data' URL copy-pasten (und geojson als Format angeben)).
- In der [resultierenden uMap](http://umap.osm.ch/m/3161/) chli rumbasteln
    - Icon rot, mit 'Drop' als Icon shape
    - Icon Symbol *nicht* mit einem Bildli versehen, sondern `{name}` (Mersi an [@das-g](https://matrix.to/#/!SKrlcOagVFDvtqOndy:matrix.org/$1638795222589825FegDE:matrix.org?via=matrix.org&via=binarylogic.ch&via=mozilla.org)).
    - In 'Interaction options' bei 'Popup content template' `Am {name}. Dezämber isch ds Adventsfänschter ar {addr:street} {addr:housenumber} {level}` einfüllen, damit die Popups bei den Icons beschreiben, in welchem Stockwerk das Adventsfenster ist, wenn wir das wissen.
- Diese uMap als iFrame in der [HTML-Datei](index.html) [schön bildschirmfüllend darstellen](https://stackoverflow.com/a/27832759/323100)
- Voila; https://wilkerstrasse.ch zeigt wo welches Adventsfenster ist.
