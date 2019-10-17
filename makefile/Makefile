JUNKFILES = .irb_history .pip .ScanSnap .nbems .fldigi .cpan
JUNKFILES += .gdb_history .mysql_history .sqlite_history
#BREWPACKAGES := mosh duplicity pv offlineimap wget nmap tor torsocks
YYYYMM := $(shell date +%Y%m)

NO_COLOR = \033[0m
O1_COLOR = \033[0;01m
O2_COLOR = \033[32;01m

PREFIX = "$(O2_COLOR)==>$(O1_COLOR)"
SUFFIX = "$(NO_COLOR)"

default: clean

cleanup:
	-mkdir -p $(HOME)/Documents/$(YYYYMM)
	-mv $(HOME)/Desktop/* $(HOME)/Documents/$(YYYYMM)

clean: cleanup
	@echo $(PREFIX) $@ $(SUFFIX)
	@-rm -rf ~/.tmp/*
	@-rm -rf ~/.Trash/*
	@-rm -rf $(JUNKFILES)
