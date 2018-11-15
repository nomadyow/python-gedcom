# Python GEDCOM Parser

[![PyPI](https://img.shields.io/pypi/v/python-gedcom.svg)](https://pypi.org/project/python-gedcom/)
[![GitHub release](https://img.shields.io/github/release/nickreynke/python-gedcom.svg)](https://github.com/nickreynke/python-gedcom/releases)
![](https://img.shields.io/badge/GEDCOM%20format%20version-5.5-yellowgreen.svg)
![](https://img.shields.io/badge/Python%20version-2%20and%203-yellowgreen.svg)

A Python module for parsing, analyzing, and manipulating GEDCOM files.

GEDCOM files contain ancestry data. The parser is currently supporting
the GEDCOM 5.5 format which is detailed [here](https://chronoplexsoftware.com/gedcomvalidator/gedcom/gedcom-5.5.pdf).

> **NOTE**: This module is currently under development and **should not be used in production**!
> The current development process can be tracked in the ["develop" branch](https://github.com/reynke/python-gedcom/tree/develop).

## Installation

> **NOTE**: As of the 26 march of 2018 the beta of the new Python Package
> Index launched. I recommend reading this: "[All New PyPI is now in beta](https://pyfound.blogspot.de/2018/03/warehouse-all-new-pypi-is-now-in-beta.html)"

The module can be installed via [pip](https://pip.pypa.io/).

Run `pip install python-gedcom` to install or `pip install python-gedcom --upgrade`
to upgrade to the newest version uploaded to the [PyPI repository](https://pypi.org/project/python-gedcom/).

## Usage

When successfully installed you may import the `gedcom` module and use
it like so:

```python
from gedcom import Gedcom

file_path = '' # Path to your `.ged` file
gedcom = Gedcom(file_path)

# Then run methods on `gedcom` ... :)
```

## History

This module was originally based on a GEDCOM parser written by 
Daniel Zappala at Brigham Young University (Copyright (C) 2005) which
was licensed under the GPL v2 and then continued by
[Mad Price Ball](https://github.com/madprime) in 2012.

## Changelog

**v0.2.1dev**

- Changed broken links to GEDCOM format specification ([#2](https://github.com/nickreynke/python-gedcom/issues/2))

**v0.2.0dev**

- Added `develop` branch to track and update current development process
- Applied PEP 8 Style Guide conventions
- **Renamed variables and methods** to make their purpose more clear
- **Outsourced GEDCOM tags to module level**
- **Added missing inline documentation**
- Optimized `README.md` (sections and better description)
- Added `LICENSE` file
- Cleaned up and optimized code

**v0.1.1dev**

- initial release; [forked](https://github.com/madprime/python-gedcom)

## License

Licensed under the [GNU General Public License v2](http://www.gnu.org/licenses/gpl-2.0.html)

**Python GEDCOM Parser**
<br>Copyright (C) 2018 Nicklas Reincke (contact at reynke.com)
<br>Copyright (C) 2016 Andreas Oberritter
<br>Copyright (C) 2012 Madeleine Price Ball
<br>Copyright (C) 2005 Daniel Zappala (zappala at cs.byu.edu)
<br>Copyright (C) 2005 Brigham Young University

This program is free software; you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation; either version 2 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License along
with this program; if not, write to the Free Software Foundation, Inc.,
51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
