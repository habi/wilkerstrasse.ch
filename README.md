# wilkerstrasse.ch

Website für den Adventskalender 2020 an der Wilkerstrasse

## HowTo

- Repository machen und in den 'Settings' einstellen, dass [GitHub Pages](https://pages.github.com) eine Webseite davon serviert.
- Bei [cyon.ch](https://www.cyon.ch/domains/) eine Domain kaufen.
- [CNAME](CNAME) in GitHub auf die neu gekaufte Domain umbiegen.
- Bei Cyon CNAME und [A-Record](https://docs.github.com/en/free-pro-team@latest/github/working-with-github-pages/managing-a-custom-domain-for-your-github-pages-site#configuring-an-apex-domain) für GitHub Pages einstellen.
- Tabelle von Andrea mit den Adventsfenstern auf [GeoJSON.io](http://geojson.io) händisch in eine [GeoJSON-Datei](https://git.io/JkdqT) umklicken.
- Diese GeoJSON-Datei in einer [uMap](https://wiki.openstreetmap.org/wiki/DE:UMap) als Datenquelle einfügen (dafür bei der [Datei hier im GitHub Repository Gist](https://github.com/habi/wilkerstrasse.ch/blob/main/adventsfenster.geojson) oben rechts auf 'Raw' klicken und [diese URL](https://raw.githubusercontent.com/habi/wilkerstrasse.ch/main/adventsfenster.geojson) nehmen).
- In der [resultierenden uMap](http://umap.osm.ch/m/3161/) chli rumbasteln, dass die Pop-Up der Marker so werden wie gedacht (d.h. `Am {name}. Dezämber isch ds Adventsfänschter ar addr:street} {addr:housenumber} {level}` in 'Popup content template' in 'Interaction options' einfüllen).
- Diese uMap als iFrame in der [HTML-Datei](index.html) [schön bildschirmfüllend darstellen](https://stackoverflow.com/a/27832759/323100)
- Voila; https://wilkerstrasse.ch ist gemacht.
