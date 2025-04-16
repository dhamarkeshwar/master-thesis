Changelog
=========
All notable changes to this project are documented in this file in reverse
chronological order of publication.

The version number corresponds to the version number of the kulemt document
class. The version number of kulemtx.sty and the prublication date of
kulemt.ini are mentionned as a comment.

The format is based on [Keep a
Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to
[Semantic Versioning](http://semver.org/spec/v2.0.0.html) since version 2.


## v2.0.0 - 2025-04-03

### Added
- Engines LuaTeX and XeTeX supported
- Option `british` selects the language variant British, which is the English
  variant preferred by the KU Leuven
- Option `twosidelrequal` implements a `twoside` layout with equal left and
  right margins
- Option `article` selects an article layout, which can be used for additional
  articles
- Option `twocolumn` can be used with the article layout
- Option `cfgfile` can be used to select another configuration file
- New master "ai" (`kulemt.ini` 2025-02-17)
- Rollback to version 1 available

### Changed
- Minimal requirements for LaTeX (2018-04-06) and for the L3 programming layer
  (2019-04-06)
- Default input encoding changed from ASCII to UTF-8
- New configuration file format and file name (`kulemt.ini`)
- Option `acyear` is a 4-digit number, no longer a range
- The default option to position the typeblock is `twosidelrequal` instead of
  `twoside`
- `kulemtx.sty` updated to version 1.0
- Copyright text updated to the KU Leuven requirements (`kulemt.ini` 2025-02-17)

### Removed
- Configuration file format of `kulemt.cfg` no longer supported
- Master specific configuration file no longer supported
- Option `filingcard` and its related options `translatedtitle`,
  `shortabstract`, `udc`, `keywords`, and `articletitle`
- Option `font`
- Option `inputenc`
- Option `bindcover`
- Option `nomicrotype`


## v1.14 - 2023-04-05

### Added
- New masters "ebwk", "mcs", "ulp" (`kulemt.cfg`)

### Changed
- Masters and options updated to the 2022 situation (`kulemt.cfg`)

### Fixed
- Uncrop faculty logo (`logokuleng.pdf`)
- Avoid \setlipsumdefault: no longer available in recent versions of
  lipsum.sty (`masterproef.tex` & `thesis.tex`)


## v1.13 - 2022-04-18

### Changed
- Masters and options updated to the 2021 situation (`kulemt.cfg`)
- Update the guidelines, manual and templates accordingly

### Fixed
- Changed titles (promoter, assessor, assistant)
  as suggested by the university (`kulemt.cfg`)


## v1.12 - 2021-09-11

### Changed
- Remove test for hyphenation patterns (`kulemt.cls`)

### Fixed
- Updated faculty logo


## v1.11 - 2021-03-11

### Added
- New master "eksuma" (`kulemt.cfg`)

### Changed
- Update the masters: "elt", "eelt" (`kulemt.cfg`)
- Changelog now in file `changes.txt`
- Source files moved to the Faculty website


## v1.10 - 2020-01-10

### Changed
- Masters and options updated to the 2020 situation (`kulemt.cfg`)
- Masters no longer require the filing card (`kulemt.cfg`)
- Update the guidelines, manual and templates accordingly


## v1.9 - 2017-05-30

### Added
- Pass the option `oldfontcommands` to memoir (`kulemt.cls`)
- Add master "evlit" (`kulemt.cfg`)

### Changed
- Update the masters: "bwk", "cws", "ecws", "mai", "vlit" (`kulemt.cfg`)


## v1.8a - 2015-06-01

### Changed
- Update Nano options and add some English masters (`kulemt.cfg`)


## v1.8 - 2015-05-05

### Fixed
- Allow for commands of other packages (e.g., cleveref) to globally
  modify local control sequences such as \@tempa (`kulemt.cls`)


## v1.7 - 2013-05-01

### Added
- Option `promoter` is an alias to option `promotor` (`kulemt.cls`)

### Changed
- Logos on front pages completely reworked due to new KU Leuven rules:
  new layout, Sedes removed, only color logos, combined logo of the
  KU Leuven and of the Faculty (`kulemt.cls`)
- Input encoding initialized to ASCII to detect other input encodings
  (`kulemt.cls`)
- Master programs can disallow master options (`kulemt.cls`)
- Master option abbreviations are either valid or obsolete
  Additionally you can specify the list of abbreviations, where one
  must be selected from, if the master requires so (`kulemt.cls`)
- Masters and options updated to the 2013 situation (`kulemt.cfg`)
- Some masters disallow master options (`kulemt.cfg`)

### Deprecated
- Option `bindcover` becomes obsolete because of new cover page layout
  (`kulemt.cls`)


## v1.6b - 2012-05-15

### Fixed
- Master title of "emtk" corrected (`kulemt.cfg`)


## v1.6 - 2012-05-13

### Added
- New option `bindcover` (`kulemt.cls`)
- Support for obsolete master options (`kulemt.cls`)

### Changed
- The environment `abstract*` has a new optional argument to specify
  the language (`kulemt.cls`)
- Missing master options generate a warning instead of an error (`kulemt.cls`)
- Masters and options updated to the 2012 situation (`kulemt.cfg`)

### Fixed
- "K.U.Leuven" replaced by "KU Leuven" (`kulemt.cls`)


## v1.5 - 2011-08-10

### Fixed
- \latinencoding is T1 only if T1 is the current encoding (`kulemt.cls`)
  This resolves a microtype error when using the default CMR fonts


## v1.4 - 2011-06-08

### Added
- The labels for promoters, assessors and assistants can be defined
  in the configuration file (`kulemt.cls`)
- Support for obsolete masters (`kulemt.cls`)

### Changed
- New master "mse" which replaces the obsolete "mvt" (`kulemt.cfg`)
- The label for promoter is changed to "thesis supervisor" and
  for assistant to "mentor" (`kulemt.cfg`)

### Fixed
- \mainmatter* works again (`kulemt.cls`)


## v1.3 - 2011-05-13

### Fixed
- Now compatible with the externalization library of tikz (`kulemt.cls`)


## v1.2 - 2010-08-03

### Changed
- Disallow empty values for the promoter keyword (`kulemt.cls`)

### Fixed
- Don't put empty fields on the front page (`kulemt.cls`)


## v1.1 - 2010-03-07

### Fixed
- Make accented characters work on the front page (`kulemt.cls`)


## v1.0 - 2010-03-02

### Added
- Initial version
