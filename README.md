One Page Agency Site für Neos CMS
=============================================

Dieses Paket beinhaltet das im [Neos CMS E-Book](https://www.mittwald.de/neos-e-book-template-entwicklung) umgesetzte
HTML5-Template *Agency* von [StartBootstrap](http://startbootstrap.com/template-overviews/agency/).
Eine Vorschau des Site-Packages befindet sich unter folgendem [Link](http://onepageagency.mittwald-demo.de).


Voraussetzungen
-------------

Aktualisierte Version für Neos 7 und 8

Installation
------------

Folgenden Block in die `composer.json` eintragen im Abschnitt `repositories`:

    "onepageagencyfork": {
      "type": "github",
      "url": "git@github.com:kitsunet/neos-onepageagency.git"
    }

Beispiel wie es dann aussehen könnte:

    "repositories": {
      "distributionPackages": {
        "type": "path",
        "url": "./DistributionPackages/*"
      },
      "onepageagency": {
        "type": "github",
        "url": "git@github.com:kitsunet/neos-onepageagency.git"
      }
    },


Composer update ausführen:

    composer update

Anschließend müssen alle bereits vorhandenen Seiten und Inhalte entfernt werden:

    ./flow site:prune

Vor Import des Site-Packages empfiehlt es sich noch einmal den Cache zu löschen:

    rm -rf Data/Temporary/*

Zum Schluss wird dann das zuvor geclonte Site-Package importiert:

    ./flow site:import Mw.OnePageAgencySite

Autor
-------

*Mw.OnePageAgencySite* wurde im Rahmen
der [Neos CMS E-Book Serie](https://www.mittwald.de/neos-e-book-template-entwicklung) von Tobias
Hüske (<t.hueske@mittwald.de>) erstellt.
Dankend wurde das unter
der [Apache License 2.0](https://github.com/mittwald/neos-onepageagency/tree/master/Resources/Public/LICENSE) stehende
HTML5-Template *Agency* von [StartBootstrap](http://startbootstrap.com/template-overviews/agency/) als Vorlage
verwendet.


Lizenz
-------

Das hier angebotene Paket ist unter der Apache License 2.0 lizensiert.
