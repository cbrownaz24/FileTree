GCC = gcc217

all: testft

clean:
	rm -f meminfo* dynarray.o path.o ft_client.o nodeFT.o ft.o *~

testft: dynarray.o path.o nodeFT.o ft.o ft_client.o
	$(GCC) -g $^ -o $@

dynarray.o: dynarray.c dynarray.h
	$(GCC) -g -c $<

path.o: path.c dynarray.h path.h a4def.h
	$(GCC) -g -c $<

ft_client.o: ft_client.c ft.h a4def.h
	$(GCC) -g -c $<

nodeFT.o: nodeFT.c dynarray.h nodeFT.h path.h a4def.h
	$(GCC) -g -c $<

ft.o: ft.c dynarray.h nodeFT.h ft.h path.h a4def.h
	$(GCC) -g -c $<
