CC=g++
CFLAGS= -g -Wall

all: proxy

proxy: proxy_server_with_cache.c
	$(CC) $(CFLAGS) -o proxy_parse.o -c proxy_parse.c -lpthread
	$(CC) $(CFLAGS) -o proxy.o -c proxy_server_with_cache.c -lpthread
	$(CC) $(CFLAGS) -o proxy_parse.o proxy proxy.o -lpthread

clean:
	rm -f proxy *.o

# tar:
# 	tar -cvzf ass1.tgz proxy_server_with_cache.c proxy_parse.c proxy_parse.h Makefile