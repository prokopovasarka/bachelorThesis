
# Changelog
All notable changes to this project will be documented in this file.
 
The format is based on [Keep a Changelog](http://keepachangelog.com/)
and this project adheres to [Semantic Versioning](http://semver.org/).

## [1.5.8] - 22. 5. 2025

Fixes of list of code listings and copyright text.

### Changed
- Vertical space in Lists of code listings between items from different chapter.
- Unification of Czech, Slovak and English copyright text.


## [1.5.7] - 13. 5. 2025

Improvements of title page spacing. 

### Changed
- Made smaller spacing between the logo and the title, and the title and the author's name, so it does not overflow when the name of the thesis is long.


## [1.5.6] - 13. 5. 2025

Added possibility to have onepage/twopage abstract. 

### Added
- \printtwopageabstract and \printonepageabstract commands, which allow printing abstracts on two or one page, respectively.

### Removed
- Removed \printabstractpage.

### Changed
- Fixed typography/overflowing of some texts.


## [1.5.5] - 5. 5. 2025

Fix of abstracts in table of content.

### Changed
- Refactoring abstract creation to simplify creation and handling.


## [1.5.4] - 5. 5. 2025

Fix of different CZE/ENG abstract pages.

### Changed
- Fixed visual style of first and second abstract page.


## [1.5.3] - 4. 5. 2025

Algorithm pseudocode numbering based on chapters.

### Changed
- Add automatic numbering base on chapters for `algorithm` environment.
- Add command for algorithm pseudocode listing.

## [1.5.2] - 4. 5. 2025

Improved title page spacing.

### Changed
- Changed title page vertical spaces.


## [1.5.1] - 4. 5. 2025

Improved title page, abstracts on separate pages.

### Changed
- Reordering title pages elements.
- Changed title page vertical spaces.
- Specialisation and study program added to title page.
- Abstracts are now on separate pages.


## [1.5.0] - 4. 5. 2025

Fix of class parameters, improved title page.

### Changed
- Reordered class parameters, so they work properly.
- CTU logo and CTU name on title page.
- Fix of docs typo.


## [1.4.5] - 25. 4. 2025

Added observation theorem.

### Added
- Added observation as a new theorem.


## [1.4.4] - 25. 4. 2025

Fix of PDF-A, footnotes.

### Changed
- Removed PDF-A keywords, which were breaking the PDF-A standard.
- Removed hyperref package, which is already included by pdfx package.
- Moved pdfx inclusion to end of cls because of clash with other packages.


## [1.4.3] - 1. 4. 2025

Fix of definition English version.

### Changed
- Fix of typo in "definition".
- Added some aux files to gitignore.


## [1.4.2] - 20. 3. 2025

Handle pdfx package warning about RGB.

### Added
- Added suppression for pdfx package warning about changing color model until they fix it.


## [1.4.1] - 19. 3. 2025

Removed obsolete option Unicode.

### Changed
- Removed Unicode option from the CTU FIT thesis class, since it was not used anymore.


## [1.4.0] - 19. 3. 2025

PDF metadata.

### Added
- Added code for generating file with PDF metadata for PDF/A.
- Added Czech and Slovak name for dissertation thesis.

### Changed
- Updated hyperref package.


## [1.3.10] - 27. 2. 2025

Darkmode image example improved.

### Changed
- New darkmode example image.
- Added citation for darkmode example image.


## [1.3.9] - 7. 1. 2025

Cleaning the bibliography.

### Changed
- Removed unused bibliography items, only example of different entries remained.
- Improved bibliography item for website citation.
- Added non-breaking spaces before citations.


## [1.3.8] - 29. 10. 2024

Gitignore improvement and attachment list improvement.

### Changed
- Add root folder to attachments list to comply with standard.
- Add pdfa.xmpi to gitignore.


## [1.3.7] - 5. 7. 2024
  
The generated PDF now complies to the PDF/A-1B standard.

### Added
- Added support code for PDF/A generation.


# [1.3.6] - 5. 7. 2024

Improved the example text.
 
### Added
- Added image with white mode/dark mode settings to show the contrast.


# [1.3.5] - 25. 6. 2024

Making .gitignore less strict when handling PDF files.
 
### Changed
- The .gitignore was made less strict, so it does not ignore every .pdf file, but just the example/output ones.


# [1.3.4] - 25. 6. 2024
  
Added support for paragraphs as the deepest level of headings via documentclass option.
 
### Added
- Added "paragraph" option for document class. If passed, it styles the paragraph command as another level of heading, adds number to it and shows it in ToC. Use with care! Normally, it is considered unwise to use it, since its too deep.


# [1.3.3] - 22. 6. 2024
  
Fixed warning about header height. Update of arara compilation settings.
 
### Fixed
- Fixed "Package fancyhdr Warning: \headheight..." warning.

### Changed
- Changed arara settings to properly match the new default compiler.


## [1.3.2] - 18. 6. 2024
  
Improvements of captions in the example.
 
### Changed
- All captions are now at the bottom of the object (figure, listing, table, etc.).
- The trailing spaces have been removed from the caption


## [1.3.1] - 17. 6. 2024
  
Improvements of frontmatter, table of contents entries and sectioning.
 
### Changed
- Changed order of front matter entries (acknowledgements, dedications, etc.) to match standard sectioning.
- Excluding frontmatter entries from table of contents.

### Fixed
- Fixed missing empty page after titlepage.
- Fixed numbering/toc of subsubsection.


## [1.3.0] - 17. 6. 2024
  
Dropped older compilers that do not support computer-read PDFs (e.g., the text could not be copy-pasted). Now, only XeLaTeX and LuaLaTeX can be used.
 
### Changed
- Changed the if that processes the used compiler, so it supports only XeLaTex or LuaLaTeX. Otherwise, error is raised.



## [1.2.2] - 17. 6. 2024
  
Title page is now first, the assignment is second page.
 
### Changed
- Swapped Title page and assignment page.



## [1.2.1] - 17. 6. 2024
  
Sync of layout for oneside and twoside versions. 
 
### Changed
- The introduction chapter is numbered (as it should have been).

### Fixed
- Fixed the problem that oneside and twoside versions had different layouts because of different margings.



## [1.2.0] - 17. 6. 2024
  
Started versioning.

### Added
- Version number of the project.
- This changelog file.
