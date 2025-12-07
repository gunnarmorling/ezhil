CSS Files Location
==================

CSS files are NOT stored in this directory (themes/ezhil/static/css/).

Location:
---------
Theme CSS source files are located in:
  /themes/ezhil/assets/css/

Files:
  - normalize.css
  - main.css
  - dark.css

Why:
----
CSS files are processed through Hugo Pipes (resources.Get) which:
1. Minifies the CSS (removes whitespace, comments)
2. Adds fingerprinting (cache-busting via content hash)
3. Serves optimized files from /resources/ directory

The Hugo Pipes processing requires files to be in the assets/ directory,
not the static/ directory. Files in static/ are copied as-is without
any processing.

To update CSS:
--------------
Edit the files in /themes/ezhil/assets/css/, then rebuild the site with
Hugo. The processed/minified versions will be automatically generated in
the /resources/ directory.
