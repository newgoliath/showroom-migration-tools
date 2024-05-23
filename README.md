= showroom-migration-tools

== Utils

Migrating from bookbag to antora

. Create a nav.adoc file from the modules.yaml file:
+
`b2s.pl`:: Converts bookbag `/workhop/modules.yaml` to antora `nav.adoc`

. Convert the % to {} in your bookbag source files:
+
`adoc_percent2brace.sh`:: For the list of vars, change the percent signs to curly braces.

. Move adoc and image files from `/workshop/content` to `modules/ROOT`.
Also resizes images and generates site.
+
CAUTION: You'll have to edit this file for paths, etc.
+
`move_files_and_generate.sh`:: Move files adoc from old directory to new directory, resize images and generate site.

== Other Stuff
`freeform-playbook.yml`:: An anotra "playbook", just an exmaple
`bookbag2showroom.adoc`:: Design document for `/workshop/modules.yaml` to `nav.adoc`
