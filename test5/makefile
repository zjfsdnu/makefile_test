test:
    # 这是测试
	@echo "hello"

txt = Hello World
test2:
	@echo $(txt)

test3:
	@echo $$HOME

a.txt b.txt: 
	@touch $@

a1.txt: b.txt c.txt
	cp $< $@ 

dest/%.txt: src/%.txt
	@[ -d dest ] || mkdir dest
	cp $< $@
