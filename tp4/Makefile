CFLAGS ?= -pedantic -g -O2 -std=c11 -Wall -Wextra -Wvla
LDFLAGS := -lm

OBJS = cachesim.o cache_simulator.o metric_counter.o

cachesim: $(OBJS)

metric_counter.o: metric_counter.c
cache_simulator.o: cache_simulator.c metric_counter.c
cachesim.o: cache_simulator.c

clean:
	rm -f $(OBJS) cachesim

.PHONY: clean