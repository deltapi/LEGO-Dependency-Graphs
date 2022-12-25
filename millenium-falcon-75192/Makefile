OBJS := $(wildcard ./*.dot)

all: $(OBJS:.dot=.pdf) $(OBJS:.dot=.eps)

%.pdf: %.dot
	mkdir -p pdf
	dot -Tpdf -o pdf/$@ $<

%.eps: %.dot
	mkdir -p eps
	dot -Teps -o eps/$@ $<

clean:
	rm -rf $(BUILDDIRS)
