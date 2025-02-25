Release History
===============

5.0.0 (2021-11-26)
------------------
* Fix a typo in HISTORY.rst (#904 by @TurnrDev)

* Fix typo and fix return value written in docstrings (#903 by @rariyama)

* Add deprecation warning for delete_row method in documentation (#909 by @javad94)

* split files `models.py` and `test.py` (#912 by @lavigne958)

* parent 39d1ecb59ca3149a8f46094c720efab883a0dc11 author Christian Clauss <cclauss@me.com> 1621149013 +0200 commit
ter Christian Clauss <cclauss@me.com> 1630103641 +0200 (#869 by @cclaus)

* Enable code linter in CI (#915 by @lavigne958)

* isort your imports (again), so you don't have to (#914 by @cclaus)

* lint_python.yml: Try 'tox -e py' to test current Python (#916 by @cclaus)

* Add more flake8 tests (#917 by @cclaus)

* Update test suite (#918 by @cclaus)

* Avoid IndexError when row_values() returns an empty row (#920 by @cclaus)

* Bugfix - remove wrong argument in `batch_update` docstring (#912 by @lavigne958)

* Improvement - Add `Worksheet.index` property (#922 by @lavigne958)

* Add ability to create directory if it does not exist before saving the credentials to disk. (#925 by @benhoman)

* Update test framework and VCR and cassettes (#926 by @lavigne958)

* Delete .travis.yml (#928 by @cclaus)

* Update tox.ini with all linting commands under lint env (by @lavigne958)

* Build package and docs in CI (#930 by @lavigne958)

* Update oauth2.rst (#933 by @amlestin)

* Update the link to the Google Developers Console (#934 by @Croebh)

* allow tests to run on windows, add and improve tests in WorksheetTests, add test on unbounded range,
  use canonical range as specified in the API, add test cassettes, prevent InvalidGridRange,
  improve code formatting (#937 by @Fendse)

* fix fully qualified class names in API documentation (#944 by @geoffbeier)

* fix editor_users_emails - get only from list not all users added to spreadsheet (#939 by @Lukasz)

* add shadow method to get a named range from a speadsheet instance (#941 by @lavigne958)

* auto_resize_columns (#948 by @FelipeSantos75)

* add functions for defining, deleting and listing named ranges (#945 by @p-doyle)

* Implement `open` sheet within Drive folder (#951 by @datavaluepeople)

* Fix get range for unbounded ranges (#954 by @lavigne958)

* remove potential I/O when reading spreadsheet title (956 by @lavigne958)

* Add include_values_in_response to append_row & append_rows (#957 by @martimarkov)

* replace raw string "ROWS" & "COLUMNS" to Dimension named tuple,
  replace raw string "FORMATTED_VALUE", "UNFORMATTED_VALUE", "FORMULA" to ValueRenderOption named tuple,
  replace raw string "RAW", "USER_ENTERED" to ValueInputOption named tuple (#958 by @ccppoo)

4.0.1 (2021-08-07)
------------------

* Do not overwrite original value when trying to convert to a number (#902 by @lavigne958)


4.0.0 (2021-08-01)
------------------

* Changed `Worksheet.find()` method returns `None` if nothing is found (#899 by @GastonBC)

* Add `Worksheet.batch_clear()` to clear multiple ranges. (#897 by @lavigne958)

* Fix `copy_permission` argument comparison in `Client.copy()` method (#898 by @lavigne958)

* Allow creation of spreadhsheets in a shared drive (#895 by @lavigne958)

* Allow `gspread.oauth()` to accept a custom credential file (#891 by @slmtpz)

* Update `tox.ini`, remove python2 from env list (#887 by @cclaus)

* Add `SpreadSheet.get_worksheet_by_id()` method (#857 by @a-crovetto)

* Fix `store_credentials()` when `authorized_user_filename` is passed (#884 by @neuenmuller)

* Remove python2 (#879 by @lavigne958)

* Use `Makefile` to run tests (#883 by @lavigne958)

* Update documentation `Authentication:For End Users` using OAuth Client ID (#835 by @ManuNaEira)

* Allow fetching named ranges from `Worksheet.range()` (#809 by @agatti)

* Update README to only mention python3.3+ (#877 by @lavigne958)

* Fetch `creation` and `lastUpdate` time from `SpreadSheet` on open (#872 by @lavigne958)

* Fix bug with `Worksheet.insert_row()` with `value_input_option` argument (#873 by @elijabesu)

* Fix typos in doc and comments (#868 by @cclauss)

* Auto cast numeric values from sheet cells to python int or float (#866 by @lavigne958)

* Add `Worksheet.get_values()` method (#775 by @burnash)

* Allow `gspread.oauth()` to accept a custom filename (#847 by @bastienboutonnet)

* Document dictionary credentials auth (#860 by @dmytrostriletskyi)

* Add `Worksheet.get_note()` (#855 by @water-ghosts )

* Add steps for creating new keys (#856 by @hanzala-sohrab)

* Add `folder_id` argument to `Client.copy()` (#851 by @punnerud)

* Fix typos in docstrings (#848 by @dgilman)

3.7.0 (2021-02-18)
------------------

* Add `Worksheet.insert_note()`, `Worksheet.update_note()`, `Worksheet.clear_note()` (#818 by @lavigne958)

* Update documentation: oauth2.rst (#836 by @Prometheus3375)

* Documentation fixes (#838 by @jayeshmanani)

* Documentation fixes (#845 by @creednaylor)

* Add `Worksheet.insert_cols()` (#802 by @AlexeyDmitriev)

* Documentation fixes (#814 by @hkuffel)

* Update README.md (#811 by @tasawar-hussain)

* Add `value_render_option` parameter to `Worksheet.get_all_records()` (#776 by @damgad)

* Remove `requests` from `install_requires` (#801)

* Simplify implementation of `Worksheet.insert_rows()` (#799 by @AlexeyDmitriev)

* Add `auth.service_account_from_dict()` (#785 b7 @mahenzon)

* Fix `ValueRange.from_json()` (#791 by @erakli)

* Update documentation: oauth2.rst (#794 by @elnjensen)

* Update documentation: oauth2.rst (#789 by @Takur0)

* Allow `auth` to be `None`. Fix #773 (#774 by @lepture)


3.6.0 (2020-04-30)
------------------

* Add `Worksheet.insert_rows()` (#734 by @tr-fi)

* Add `Worksheet.copy_to()` (#758 by @JoachimKoenigslieb)

* Add ability to create a cell instance using A1 notation (#765 by @tivaliy)

* Add `auth.service_account()` (#768)

* Add Authlib usage (#552 by @lepture)


3.5.0 (2020-04-23)
------------------

* Simplified OAuth2 flow (#762)

* Fix `Worksheet.delete_rows()` index error (#760 by @rafa-guillermo)

* Deprecate `Worksheet.delete_row()` (#766)

* Scope `Worksheet.find()` to a specific row or a column (#739 by @alfonsocv12)

* Add `Worksheet.add_protected_range()` #447 (#720 by @KesterChan01)

* Add ability to fetch cell address in A1 notation (#763 by @tivaliy)

* Add `Worksheet.delete_columns()` (#761 by @rafa-guillermo)

* Ignore numericising specific columns in `get_all_records` (#701 by @benjamindhimes)

* Add option ``folder_id`` when creating a spreadsheet (#754 by @Abdellam1994)

* Add `insertDataOption` to `Worksheet.append_row()` and `Worksheet.append_rows()` (#719 by @lobatt)


3.4.2 (2020-04-06)
------------------

* Fix Python 2 `SyntaxError` in models.py #751 (#752)


3.4.1 (2020-04-05)
------------------

* Fix `TypeError` when using gspread in google colab (#750)


3.4.0 (2020-04-05)
------------------

* Remove `oauth2client` in favor of `google-auth` #472, #529 (#637 by @BigHeadGeorge)
* Convert `oauth2client` credentials to `google-auth` (#711 by @aiguofer)
* Remove unnecessary `login()` from `gspread.authorize`

* Fix sheet name quoting issue (#554, #636, #716):
    * Add quotes to worksheet title for get_all_values (#640 by @grlbrwrg, #717 by @zynaxsoft)
    * Escaping title containing single quotes with double quotes (#730 by @vijay-shanker)
    * Use `utils.absolute_range_name()` to handle range names (#748)

* Fix `numericise()`: add underscores test to work in python2 and <python3.6 (#622 by @epicfaace)

* Add `supportsAllDrives` to Drive API requests (#709 by @justinr1234)

* Add `Worksheet.merge_cells()` (#713 by @lavigne958)
* Improve `Worksheet.merge_cells()` and add `merge_type` parameter (#742 by @aiguofer)

* Add `Worksheet.sort()` (#639 by @kirillgashkov)

* Add ability to reorder worksheets #570 (#571 by @robin900)
    * Add `Spreadsheet.reorder_worksheets()`
    * Add `Worksheet.update_index()`

* Add `test_update_cell_objects` (#698 by @ogroleg)

* Add `Worksheet.append_rows()` (#556 by @martinwarby, #694 by @fabytm)

* Add `Worksheet.delete_rows()` (#615 by @deverlex)

* Add Python 3.8 to Travis CI (#738 by @artemrys)

* Speed up `Client.open()` by querying files by title in Google Drive (#684 by @aiguofer)

* Add `freeze`, `set_basic_filter` and `clear_basic_filter` methods to `Worksheet` (#574 by @aiguofer)

* Use Drive API v3 for creating and deleting spreadsheets (#573 by @aiguofer)

* Implement `value_render_option` in `get_all_values` (#648 by @mklaber)

* Set position of a newly added worksheet (#688 by @djmgit)
* Add url properties for `Spreadsheet` and `Worksheet` (#725 by @CrossNox)

* Update docs: "APIs & auth" menu deprecation, remove outdated images in oauth2.rst (#706 by @manasouza)


3.3.1 (2020-04-01)
------------------

* Support old and new collections.abc.Sequence in `utils` (#745 by @timgates42)


3.3.0 (2020-03-12)
------------------

* Added `Spreadsheet.values_batch_update()` (#731)
* Added:
    * `Worksheet.get()`
    * `Worksheet.batch_get()`
    * `Worksheet.update()`
    * `Worksheet.batch_update()`
    * `Worksheet.format()`

* Added more parameters to `Worksheet.append_row()` (#719 by @lobatt, #726)
* Fix usage of client.openall when a title is passed in (#572 by @aiguofer)


3.2.0 (2020-01-30)
------------------

* Fixed `gspread.utils.cell_list_to_rect()` on non-rect cell list (#613 by @skaparis)
* Fixed sharing from Team Drives (#646 by @wooddar)
* Fixed KeyError in list comprehension in `Spreadsheet.remove_permissions()` (#643 by @wooddar)
* Fixed typos in docstrings and a docstring type param (#690 by @pedrovhb)
* Clarified supported Python versions (#651 by @hugovk)
* Fixed the Exception message in `APIError` class (#634 by @lordofinsomnia)
* Fixed IndexError in `Worksheet.get_all_records()` (#633 by @AivanF)

* Added `Spreadsheet.values_batch_get()` (#705 by @aiguofer)


3.1.0 (2018-11-27)
------------------

* Dropped Python 2.6 support

* Fixed `KeyError` in `urllib.quote` in Python 2 (#605, #558)
* Fixed `Worksheet.title` being out of sync after using `update_title` (#542 by @ryanpineo)
* Fix parameter typos in docs (#616 by @bryanallen22)
* Miscellaneous docs fixes (#604 by @dgilman)
* Fixed typo in docs (#591 by @davidefiocco)

* Added a method to copy spreadsheets (#625 by @dsask)
* Added `with_link` attribute when sharing / adding permissions (#621 by @epicfaace)
* Added ability to duplicate a worksheet (#617)
* Change default behaviour of numericise function #499 (#502 by @danthelion)
* Added `stacklevel=2` to deprecation warnings


3.0.1 (2018-06-30)
------------------

* Fixed #538 (#553 by @ADraginda)


3.0.0 (2018-04-12)
------------------

* This version drops Google Sheets API v3 support.
    - API v4 was the default backend since version 2.0.0.
    - All v4-related code has been moved from `gspread.v4` module to `gspread` module.


2.1.1 (2018-04-08)
------------------

* Fixed #533 (#534 by @reallistic)


2.1.0 (2018-04-07)
------------------

* URL encode the range in the value_* functions (#530 by @aiguofer)
* Open team drive sheets by name (#527 by @ryantuck)


2.0.1 (2018-04-01)
------------------

* Fixed #518
* Include v4 in setup.py
* Fetch all spreadsheets in Spreadsheet.list_spreadsheet_files (#522 by @aiguofer)


2.0.0 (2018-03-11)
------------------

* Ported the library to Google Sheets API v4.

  This is a transition release. The v3-related code is untouched,
  but v4 is used by default. It is encouraged to move to v4 since
  the API is faster and has more features.

  API v4 is a significant change from v3. Some methods are not
  backward compatible, so there's no support for this compatibility
  in gspread either.

  These methods and properties are not supported in v4:

  * `Spreadsheet.updated`
  * `Worksheet.updated`
  * `Worksheet.export()`
  * `Cell.input_value`


0.6.2 (2016-12-20)
------------------

* Remove deprecated HTTPError

0.6.1 (2016-12-20)
------------------

* Fixed error when inserting permissions #431

0.6.0 (2016-12-15)
------------------

* Added spreadsheet sharing functionality
* Added csv import
* Fixed bug where list of sheets isn't cleared on refetch
  #429, #386


0.5.1 (2016-12-12)
------------------

* Fixed a missing return value in `utils.a1_to_rowcol`
* Fixed url parsing in `Client.open_by_url`
* Added `updated` property to `Spreadsheet` objects


0.5.0 (2016-12-12)
------------------

* Added method to create blank spreadsheets #253
* Added method to clear worksheets #156
* Added method to delete a row in a worksheet #337
* Changed `Worksheet.range` method to accept integers as coordinates #142
* Added `default_blank` parameter to `Worksheet.get_all_records` #423
* Use xml.etree.cElementTree when available to reduce memory usage #348
* Fixed losing input_value data from following cells in `Worksheet.insert_row` #338
* Deprecated `Worksheet.get_int_addr` and `Worksheet.get_addr_int`
  in favour of `utils.a1_to_rowcol` and `utils.rowcol_to_a1` respectively


0.4.1 (2016-07-17)
------------------

* Fix exception format to support Python 2.6


0.4.0 (2016-06-30)
------------------

* Use request session's connection pool in HTTPSession

* Removed deprecated ClientLogin


0.3.0 (2015-12-15)
------------------

* Use Python requests instead of the native HTTPConnection object

* Optimized row_values and col_values

* Optimized row_values and col_values
  Removed the _fetch_cells call for each method. This eliminates the
  adverse effect on runtime for large worksheets.

  Fixes #285, #190, #179, and #113

* Optimized row_values and col_values
  Removed the _fetch_cells call for each method. This eliminates the
  adverse effect on runtime for large worksheets.

  Fixes #285, #190, #179, and #113

* Altered insert_row semantics to utilize range
  This avoids issuing one API request per cell to retrieve the Cell
  objects after the insertion row. This provides a significant speed-up
  for insertions at the beginning of large sheets.

* Added mock tests for Travis (MockSpreadsheetTest)

* Fixed XML header issue with Python 3

* Fixed Worksheet.export function and associated test

* Added spreadsheet feed helper

* Add CellNotFound to module exports
  Fixes #88

* Fixed utf8 encoding error caused by duplicate XML declarations
* Fixed AttributeError when URLError caught by HTTPError catch block
  Fixes #257

* Added __iter__ method to Spreadsheet class

* Fixed export test
* Switched tests to oauth

0.2.5 (2015-04-22)
------------------

* Deprecation warning for ClientLogin #210
* Redirect github pages to ReadTheDocs
* Bugfixes

0.2.4 (2015-04-17)
------------------

* Output error response #219 #170 #194.
* Added instructions on how to get oAuth credentials to docs.

0.2.3 (2015-03-11)
------------------

* Fixed issue with `Spreadsheet.del_worksheet`.
* Automatically refresh OAuth2 token when it has expired.
* Added an `insert_row` method to `Worksheet`.
* Moved docs to Read The Docs.
* Added the `numeric_value` attribute to `Cell`.
* Added title property to `Spreadsheet`.
* Support for exporting worksheets.
* Added row selection for keys in `Worksheet.get_all_records`.

0.2.2 (2014-08-26)
------------------

* Fixed version not available for read-only spreadsheets bug

0.2.1 (2014-05-10)
------------------

* Added OAuth2 support
* Fixed regression bug #130. Not every POST needs If-Match header

0.2.0 (2014-05-09)
------------------

* New Google Sheets support.
* Fixed get_all_values() on empty worksheet.
* Bugfix in get_int_addr().
* Changed the HTTP connectivity from urllib to httlib for persistent http connections.

0.1.0 (2013-07-09)
------------------

* Support for deleting worksheets from a spreadsheet.

0.0.15 (2013-02-01)
------------------

* Couple of bugfixes.

0.0.14 (2013-01-31)
------------------

* Bugfix in Python 3.


0.0.12 (2011-12-25)
------------------

* Python 3 support.


0.0.9 (2011-12-16)
------------------

* Enter the Docs.
* New skinnier login method.


0.0.7 (2011-12-14)
------------------

* Pypi install bugfix.


0.0.6 (2011-12-13)
------------------

* Batch cells update.


0.0.2 (2011-12-12)
------------------

* New spreadsheet open methods:

    - Client.open_by_key
    - Client.open_by_url


0.0.1 (2011-12-12)
------------------

* Got rid of the wrapper.
* Support for pluggable http session object.


pre 0.0.1 (2011-12-02)
----------------------

* Hacked a wrapper around Google's Python client library.
