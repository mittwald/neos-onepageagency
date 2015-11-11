One Page Agency Site für Neos CMS
=============================================

Dieses Paket beinhaltet das im [Neos CMS E-Book](https://www.mittwald.de/neos-e-book-template-entwicklung) umgesetzte HTML5-Template *Agency* von [StartBootstrap](http://startbootstrap.com/template-overviews/agency/).
Eine Vorschau des Site-Packages befindet sich unter folgendem [Link](http://onepageagency.mittwald-demo.de).


Voraussetzungen
-------------

Das Site-Package wurde mit Neos CMS in Version 2.x entwickelt.

    "require": {
        "typo3/neos": "2.*",
        "typo3/neos-nodetypes": "*"
    }


Installation
------------

In den Root-Ordner der Neos-Installation wechseln:
     
    cd /var/www/your-neos

Code von GitHub in den Ordner *Packages/Sites* der Neos-Installation clonen:

    git clone https://github.com/mittwald/neos-onepageagency.git Packages/Sites/Mw.OnePageAgencySite
    
Anschließend müssen alle bereits vorhandenen Seiten und Inhalte entfernt werden:
    
    ./flow site:prune
    
Vor Import des Site-Packages empfiehlt es sich noch einmal den Cache zu löschen:
    
    rm -rf Data/Temporary/*
    
Zum Schluss wird dann das zuvor geclonte Site-Package importiert:
    
    ./flow site:import Mw.OnePageAgencySite
    

Autor
-------

*Mw.OnePageAgencySite* wurde im Rahmen der [Neos CMS E-Book Serie](https://www.mittwald.de/neos-e-book-template-entwicklung) von Tobias Hüske (<t.hueske@mittwald.de>) erstellt. 
Dankend wurde das unter der [Apache License 2.0](https://github.com/mittwald/neos-onepageagency/tree/master/Resources/Public/LICENSE) stehende HTML5-Template *Agency* von [StartBootstrap](http://startbootstrap.com/template-overviews/agency/) als Vorlage verwendet.


Lizenz
-------

Das hier angebotene Paket ist unter der Apache License 2.0 lizensiert.