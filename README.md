# crosstowntrail-web
Crosstown Trail website bits


To generate the cue sheet sub-website, install mkdocs and run it.

> pip install mkdocs-pdf-export-plugin

The mkdocs-pdf-export-plugin contains all dependencies needed except for Cairo...
You'll need to read the docs to install GTK for that. See the Weasyprint instructions.
Possibly run gtk2r-env.bat


To build the cue-sheet part of the website

> mkdocs build

Then upload the contents of the 'site/cue-sheets' directory to the /resources/cue-sheets section of the website.


## How Translation works:
Since mkdocs doesn't have native 'translation' support, and we're not using any wrappers/plugins,
and since the system is really set up to use external links from the main website instead
of internal links... the translations are done by simply creating a new file with a new name.
This means that some of the headings, etc are in English. It's not really conceptually connected.
