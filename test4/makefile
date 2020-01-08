var-lost:
	export foo=ba
	echo "foo=[$$foo]"

var-kept:
	@export foo=bar; \
	echo "foo=[$$foo]"; \
	echo "[aa$$foo]"

.ONESHELL:
var-kept2:
	export foo=bar1
	echo "foo=[$$foo]"

