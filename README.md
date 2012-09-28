Installatie
============

1. Run in deze map het volgende commando:

  `bundle install`


Gebruik
============

Om het bestand genaamd groningen.kml te parsen run je het volgende commando:

  `bin/parse -s ./kml/groningen.kml -d ./output/groningen.py -t ./templates/django.mustache`

Dit commando zal de file `groningen.kml` parsen en vervolgens door het template genaamd `django.mustache` gehaald worden. Het bestand dat hier uit komt wordt opgeslagen in `groningen.py` in de output map.

Voor meer vragen over `bin/parse` kan je ook runnen:

  `bin/parse --help`

Voor een lijst van beschikbare commando's


Buurten
============

Elke buurt heeft in de mustache templates beschikking over de volgende gegevens:

1. bu_code: De buurtcode
2. bu_naam: De buurtnaam
3. gm_naam: De gemeentenaam
4. wk_code: De wijkcode
5. gm_code: De gemeentecode

Deze variabelen kunnen als volgt opgehaald worden:

`{{bu_code}}`


Mustache
============

Voor meer vragen over Mustache, zie documentatie:

https://github.com/defunkt/mustache
