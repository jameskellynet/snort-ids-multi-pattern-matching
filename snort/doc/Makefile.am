## $Id: Makefile.am,v 1.29 2006/01/24 17:21:03 ssturges Exp $
AUTOMAKE_OPTIONS=foreign no-dependencies

EXTRA_DIST = AUTHORS NEWS BUGS README \
CREDITS \
snort_manual.pdf snort_manual.tex INSTALL USAGE \
README.alert_order \
README.asn1 \
README.csv \
README.database \
README.event_queue \
README.FLEXRESP \
README.FLEXRESP2 \
README.flow \
README.flowbits \
README.flow-portscan \
README.frag3 \
README.ftptelnet \
README.http_inspect \
README.INLINE \
README.PerfProfiling \
README.PLUGINS \
README.sfportscan \
README.SMTP \
README.thresholding \
README.UNSOCK \
README.WIN32 \
README.wireless \
snort_schema_v106.pdf \
PROBLEMS RULES.todo WISHLIST faq.pdf faq.tex

DISTCLEANFILES= snort_manual.log snort_manual.toc snort_manual.aux faq.log faq.toc faq.aux snort_manual.pdf faq.pdf snort_manual.out

doc_DIR = $(prefix)/doc

SUFFIXES = .tex .dvi .ps

.tex.dvi:
	pslatex $< && pslatex $< && pslatex $<

.dvi.ps:
	dvips $< -o

.ps.pdf:
	ps2pdf $<

# perhaps one day, we will have a Makefile in the signatures directory...
# SUBDIRS = signatures
