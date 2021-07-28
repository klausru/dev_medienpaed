# dev_medienpaed
Development documentation of https://www.medienpaed.com. MedienPädagogik. Zeitschrift für Theorie und Praxis der Medienbildung

The general advice is not to touch or change the core unless via pull requests to https://github.com/pkp/ojs and https://github.com/pkp/pkp-lib/ . This maintains upgrade compatibility. Code development for individual installations shall be done within its theme and through plugins. Please share your ```code``` and please contribute to original repositories!


## The core
* Current OJS Version: 3.2.1.3 -> https://pkp.sfu.ca/ojs/download/ojs-3.2.1-3.tar.gz
* Preparing for latest OJS Version: 3.3.0.7 -> https://pkp.sfu.ca/ojs/download/ojs-3.3.0-7.tar.gz


## The theme
* https://github.com/klausru/medienpaed_hs (based on https://github.com/pkp/healthSciences with intensive modification)


### Some tricks and features
* Supports Videoabstracts. Videofiles uploaded as "videoabstract" will be displayed on the landing page
* fully responsive, built with flex divs, order divs for mobile view by ranking
* semi-generative SVG issue covers built with https://github.com/processing/p5.js and https://github.com/zenozeng/p5.js-svg

## The plugins


### activated from stock
(list rather those NOT to be activated such as payment, URN, ...)


### installed from plugin gallery
* COinS
* QuickSubmit
* Matomo
* AddThis
* Custom Header Plugin
* Custom Locale Plugin
* JATS Template Plugin (probably not needed)
* OAI JATS Plugin
* Manuscript (Default child theme) -> Download only, do not activate
* Texture plugin
* Crossref Reference Linking Plugin
* ORCiD Profile
* OpenAIRE Plugin 2.0
* Text Editor Extras
* PKP|PN (PKP Preservation Network) Plugin


### from github (via git pull)
* https://github.com/klausru/announcementEmail
* https://github.com/klausru/themeIssues
* https://github.com/klausru/dissertations
* https://github.com/klausru/jahrbuch
* https://github.com/klausru/JATSParserPlugin -> locale/de_DE
* https://github.com/klausru/dnb
* https://github.com/klausru/browseBySection


### from github via release
* https://github.com/klausru/JATSParserPlugin
