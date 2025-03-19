obj-m := xdma.o
xdma-objs := libxdma.o xdma_cdev.o cdev_ctrl.o cdev_events.o cdev_sgdma.o cdev_xvc.o cdev_bypass.o xdma_mod.o xdma_thread.o

KVERSION := $(shell uname -r)

all:
        $(MAKE) -C /lib/modules/$(KVERSION)/build M=$(PWD) modules

clean:
        $(MAKE) -C /lib/modules/$(KVERSION)/build M=$(PWD) clean
