# dev_medienpaed
Development documentation of https://www.medienpaed.com. MedienPädagogik. Zeitschrift für Theorie und Praxis der Medienbildung

The general advice is not to touch or change the core unless via pull requests to https://github.com/pkp/ojs and https://github.com/pkp/pkp-lib/ . This maintains upgrade compatibility. Code development for individual installations shall be done within its theme and through plugins. Please share your ```code``` and please contribute to original repositories!


## The core
* Current OJS Version: 3.3.0.7 -> https://pkp.sfu.ca/ojs/download/ojs-3.3.0-7.tar.gz
* Past OJS Version: 3.2.1.3 -> https://pkp.sfu.ca/ojs/download/ojs-3.2.1-3.tar.gz


## The theme
* https://github.com/klausru/medienpaed_hs (based on https://github.com/pkp/healthSciences with intensive modification)


### Some tricks and features
* Supports Videoabstracts. Videofiles uploaded as "videoabstract" will be displayed on the landing page
* fully responsive, built with flex DIVs, order DIVs for mobile view by ranking
* supports "missing covers" (future dev is to generate a SVG from the first page of the article PDF. [See the thread in the PKP forum](https://forum.pkp.sfu.ca/t/automatically-generate-article-covers-thumbnails-from-pdf/65217)

* Fully generative SVG Issue covers. Just add a <svg> background. Content will be retrieved from database. Plugin is in development

* Alternatively: semi-generative SVG issue covers (will be uploaded and live shortly) built with https://github.com/processing/p5.js and https://github.com/zenozeng/p5.js-svg
  * Version mountains is based on https://github.com/anokhee/generative-landscapes/blob/master/p5js-version/index.js
  * Version waves is based or inspired by https://openprocessing.org/sketch/977554
  * colorsets generated through curl and API via http://colormind.io/api-access/

## The plugins


### activated from stock
(list rather those NOT to be activated such as payment, URN, ...)


### installed from plugin gallery
* COinS
* QuickSubmit
* Matomo
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
* PKP|PN (PKP Preservation Network) Plugin -> Not working yet. When activated, it kills the plugin and custom locale page in the dashboard. See forum)


### from github (via git pull)
* https://github.com/klausru/announcementEmail
* https://github.com/klausru/themeIssues
* https://github.com/klausru/dissertations
* https://github.com/klausru/jahrbuch
* https://github.com/klausru/JATSParserPlugin -> locale/de_DE
* https://github.com/klausru/dnb (don't PR changes yet. We need our own filters for diposits)
* https://github.com/klausru/browseBySection
* https://github.com/klausru/addThis (initially forked, but we need our own adjustments)


### from github via release
* https://github.com/klausru/JATSParserPlugin
