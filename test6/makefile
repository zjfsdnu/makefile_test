ifeq ($(CC),gcc)
	libs=$(libs_for_gcc)
else
	libs=$(normal_libs)
endif

LIST = one two three
all:
	@for i in $(LIST); do \
		echo $$i; \
	done