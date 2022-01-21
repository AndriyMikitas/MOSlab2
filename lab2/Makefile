EXE=01-allocating-memory 02-reading-files 03-ipc 04-exec 04-payload 05-sockets-fd-smph

.PHONY: all
all: $(EXE)

04-payload: 04-payload.asm
	nasm -o 04-payload 04-payload.asm

%: %.c
	gcc -Wall -ggdb -o $@ $< -pthread

.PHONY: clean
clean:
	rm -rfv $(EXE)
