#

dist_man_MANS = \
	varnish-cli.7 \
	varnish-counters.7 \
	vcl.7 \
	vsl.7 \
	vsl-query.7 \
	varnishadm.1 \
	varnishd.1 \
	varnishhist.1 \
	varnishlog.1 \
	varnishncsa.1 \
	varnishstat.1 \
	varnishtest.1 \
	vtc.7 \
	varnishtop.1 \
	vmod_directors.3 \
	vmod_std.3

CLEANFILES = $(dist_man_MANS)

RST2ANY_FLAGS = --halt=2

varnish-cli.7: $(top_srcdir)/doc/sphinx/reference/varnish-cli.rst
	${RST2MAN} $(RST2ANY_FLAGS) $(top_srcdir)/doc/sphinx/reference/varnish-cli.rst $@

varnish-counters.7: $(top_srcdir)/doc/sphinx/reference/varnish-counters.rst
	${RST2MAN} $(RST2ANY_FLAGS) $(top_srcdir)/doc/sphinx/reference/varnish-counters.rst $@

vcl.7: $(top_srcdir)/doc/sphinx/reference/vcl.rst \
	$(top_srcdir)/bin/varnishd/builtin.vcl
	${RST2MAN} $(RST2ANY_FLAGS) $(top_srcdir)/doc/sphinx/reference/vcl.rst $@

vsl.7: $(top_srcdir)/doc/sphinx/reference/vsl.rst \
	$(top_builddir)/doc/sphinx/include/vsl-tags.rst
	${RST2MAN} $(RST2ANY_FLAGS) $(top_srcdir)/doc/sphinx/reference/vsl.rst $@

vsl-query.7: $(top_srcdir)/doc/sphinx/reference/vsl-query.rst
	${RST2MAN} $(RST2ANY_FLAGS) $(top_srcdir)/doc/sphinx/reference/vsl-query.rst $@

varnishadm.1: $(top_srcdir)/doc/sphinx/reference/varnishadm.rst
	${RST2MAN} $(RST2ANY_FLAGS) $(top_srcdir)/doc/sphinx/reference/varnishadm.rst $@

varnishd.1: \
	$(top_srcdir)/doc/sphinx/reference/varnishd.rst \
	$(top_builddir)/doc/sphinx/include/params.rst
	${RST2MAN} $(RST2ANY_FLAGS) $(top_srcdir)/doc/sphinx/reference/varnishd.rst $@

varnishncsa.1: \
	$(top_srcdir)/doc/sphinx/reference/varnishncsa.rst \
	$(top_builddir)/doc/sphinx/include/varnishncsa_options.rst \
	$(top_builddir)/doc/sphinx/include/varnishncsa_synopsis.rst
	${RST2MAN} $(RST2ANY_FLAGS) $(top_srcdir)/doc/sphinx/reference/varnishncsa.rst $@

varnishlog.1: \
	$(top_srcdir)/doc/sphinx/reference/varnishlog.rst \
	$(top_builddir)/doc/sphinx/include/varnishlog_options.rst \
	$(top_builddir)/doc/sphinx/include/varnishlog_synopsis.rst
	${RST2MAN} $(RST2ANY_FLAGS) $(top_srcdir)/doc/sphinx/reference/varnishlog.rst $@

varnishstat.1: $(top_srcdir)/doc/sphinx/reference/varnishstat.rst \
	$(top_builddir)/doc/sphinx/include/varnishstat_options.rst \
	$(top_builddir)/doc/sphinx/include/varnishstat_synopsis.rst
	${RST2MAN} $(RST2ANY_FLAGS) $(top_srcdir)/doc/sphinx/reference/varnishstat.rst $@

varnishtest.1: $(top_srcdir)/doc/sphinx/reference/varnishtest.rst
	${RST2MAN} $(RST2ANY_FLAGS) $(top_srcdir)/doc/sphinx/reference/varnishtest.rst $@

vtc.7: $(top_srcdir)/doc/sphinx/reference/vtc.rst \
	$(top_srcdir)/doc/sphinx/include/vtc-syntax.rst
	${RST2MAN} $(RST2ANY_FLAGS) $(top_srcdir)/doc/sphinx/reference/vtc.rst $@

varnishtop.1: \
	$(top_srcdir)/doc/sphinx/reference/varnishtop.rst \
	$(top_builddir)/doc/sphinx/include/varnishtop_options.rst \
	$(top_builddir)/doc/sphinx/include/varnishtop_synopsis.rst
	${RST2MAN} $(RST2ANY_FLAGS) $(top_srcdir)/doc/sphinx/reference/varnishtop.rst $@

varnishhist.1: \
	$(top_srcdir)/doc/sphinx/reference/varnishhist.rst \
	$(top_builddir)/doc/sphinx/include/varnishhist_options.rst \
	$(top_builddir)/doc/sphinx/include/varnishhist_synopsis.rst
	${RST2MAN} $(RST2ANY_FLAGS) $(top_srcdir)/doc/sphinx/reference/varnishhist.rst $@

vmod_std.3: $(top_builddir)/lib/libvmod_std/vmod_std.man.rst
	${RST2MAN} $(RST2ANY_FLAGS) $? $@

vmod_directors.3: $(top_builddir)/lib/libvmod_directors/vmod_directors.man.rst
	${RST2MAN} $(RST2ANY_FLAGS) $? $@

.NOPATH: $(dist_man_MANS)
