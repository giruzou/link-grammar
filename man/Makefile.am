
## Process this file with automake to produce Makefile.in.

man_MANS =  link-parser.1
dist_man_MANS = link-parser.man1

# Change the system dictionary location according the configuration options.
# This tracks --datadir.
link-parser.1: link-parser.man1
	sed 's,%DATA_DIR%,$(datadir),' $< >$@

clean-local:
	-rm -f link-parser.1
