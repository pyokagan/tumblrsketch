================================
Sketch Tumblr Export Workspace
================================

This workspace aims to facilitate the workflow of scanning the sketches and
automatically uploading them to pyokagan.tumblr.com in a 
rate-limited manner.

Directory Structure
=====================

* scans/ - Raw scanned images from the scanner goes here. The `scan` script
  in root can be invoked to scan images.
* complete/ - Raw scanned images which have been completed (all images extracted)
  go here. Run the `flush` script in the root directory to flush all scans into
  complete.
* in/ - Cropped and leveled and cleaned-up images go here (probably in xcf form).
  Images are removed once converted.
* out/ - Convert all images into jpgs from in, ready to be uploaded to tumblr. 
  Images are removed once uploaded.
* record/ - Record of how many images were uploaded per day.
