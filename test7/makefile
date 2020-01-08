srcfiles := $(shell echo src/{00..99}.txt)

$(subst ee,EE,feet on the street)

comma:= ,
empty:=
# space变量用两个空变量作为标识符，当中是一个空格
space:= $(empty) $(empty)
foo:= a b c
bar:= $(subst $(space),$(comma),$(foo))
# bar is now `a,b,c'.

$(patsubst %.c,%.o,x.c.c bar.c)

min: $(OUTPUT:.js=.min.js)

