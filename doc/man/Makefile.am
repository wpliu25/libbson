CLEANFILES += $(wildcard doc/man/*.3) doc/man/.doctrees doc/man/.buildinfo

.PHONY: doc/man

dist_man_MANS = $(wildcard doc/man/*.3)

man3_MANS = $(wildcard doc/man/*.3)


# sphinx-build "-E" is "ignore cache", "b" is build type.
doc/man:
	-mkdir -p doc/man
	$(SPHINX_BUILD) -qEW -b man $(top_srcdir)/doc doc/man

EXTRA_DIST += doc/man
