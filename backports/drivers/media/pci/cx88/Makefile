cx88xx-objs	:= cx88-cards.o cx88-core.o cx88-i2c.o cx88-tvaudio.o \
		   cx88-dsp.o cx88-input.o
cx8800-objs	:= cx88-video.o cx88-vbi.o
cx8802-objs	:= cx88-mpeg.o

obj-$(CONFIG_BACKPORT_VIDEO_CX88) += cx88xx.o cx8800.o
obj-$(CONFIG_BACKPORT_VIDEO_CX88_MPEG) += cx8802.o
obj-$(CONFIG_BACKPORT_VIDEO_CX88_ALSA) += cx88-alsa.o
obj-$(CONFIG_BACKPORT_VIDEO_CX88_BLACKBIRD) += cx88-blackbird.o
obj-$(CONFIG_BACKPORT_VIDEO_CX88_DVB) += cx88-dvb.o
obj-$(CONFIG_BACKPORT_VIDEO_CX88_VP3054) += cx88-vp3054-i2c.o

ccflags-y += -I$(backport_srctree)/drivers/media/i2c
ccflags-y += -I$(backport_srctree)/drivers/media/tuners
ccflags-y += -I$(backport_srctree)/drivers/media/dvb-core
ccflags-y += -I$(backport_srctree)/drivers/media/dvb-frontends
