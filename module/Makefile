LINUX_DIR ?= /lib/modules/$(shell uname -r)/build

obj-m += pteditor.o
ccflags-y += -Wno-unused-result

all:
	make -C $(LINUX_DIR) M=$(PWD) modules
clean:
	make -C $(LINUX_DIR) M=$(PWD) clean
