ALL_YML := $(wildcard *.yml)
ALL_TEST := $(patsubst %.yml,%.test,$(ALL_YML))

all : $(ALL_TEST)

%.test : %.yml
	./testwimboot $(ARGS) $<

clean :
	$(RM) in/*.ipxe in/*.txt
	$(RM) out/*.log out/*.png
