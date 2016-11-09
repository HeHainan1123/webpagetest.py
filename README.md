# webpagetest.py

## Overview

Command line utility to schedule tests at WebPageTest.org

See https://sites.google.com/a/webpagetest.org/docs/advanced-features/webpagetest-restful-apis for additional information

## Installation

- Python pypi - https://pypi.python.org/pypi/webpagetest
- Install - `pip install webpagetest`
- Create a config - `wpt --config config.json`
- Edit the config file `config.json`
    - You will need an API key from http://www.webpagetest.org/getkey.php
    - The API key is limited to 200 page loads per day. Each run, first or repeat view counts as a page load (10 runs, first and repeat view would be 20 page loads)
- Run - `wpt config.json`


## Development

- `cp config.sample.json config.json` - Create and edit a config file.
- `make` - Installs python packages.
- `make install` - Installs current git repo as a local module.
- `make run` - Runs the package supplying a config.json argument.
