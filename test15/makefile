all:
	@echo 正在编译 XXX 模块......

str: sources := foo.c bar.c baz.s ugh.h
str: objects = foo.o bar.o baz.o
str:
	@echo $(subst ee,EE,feet on the street)
	@echo $(patsubst %.c,%.o,x.c.c bar.c)
	@echo $(patsubst %.o,%.c,$(objects))
	@echo $(objects:.o=.c)
	@echo $(strip a b c )
	@echo $(findstring a,a b c)
	@echo $(findstring a,b c)
	@echo $(filter %.c %.s,$(sources))
	@echo $(sort foo bar lose)
	@echo $(word 2, foo bar baz)
	@echo $(wordlist 2, 3, foo bar baz)
	@echo $(word $(words $(sources)),$(sources))
	@echo $(firstword foo bar)
	@echo  $(patsubst %,-I%,$(subst :, ,$(VPATH)))


dir:
	@echo $(dir src/foo.c hacks)
	@echo $(notdir src/foo.c hacks)
	@echo $(suffix src/foo.c src-1.0/bar.c hacks)
	@echo $(basename src/foo.c src-1.0/bar.c hacks)
	@echo $(addsuffix .c,foo bar)
	@echo $(addprefix src/,foo bar)
	@echo $(join aaa bbb,111 222 333)

foreach: names := a b c d
foreach:
	@echo $(foreach n,$(names),$(n).o)

call: reverse = dd$(1) $(2)bb
call:
	@echo $(call reverse,a,b)

bletch = aa
ifdef bletch
	ifeq "$(origin PATH)" "environment"
		bletch = barf, gag, etc.
	endif
endif
origin:
	@echo $(bletch)

shell:
	@echo $(shell cat foo)
	@echo $(shell echo *.c)

ifdef ERROR_001
	$(error error is $(ERROR_001))
endif

ERR = $(error found an error!)

.PHONY: err

err: $(ERR)

