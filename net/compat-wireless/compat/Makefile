#ifeq ($(STERICSSON_WLAN_BUILT_IN),y)

EXTRA_CFLAGS +=  \
        -DCOMPAT_BASE_TREE="\"wl12xx.git\"" \
        -DCOMPAT_BASE_TREE_VERSION="\"v2.6.39-1250-g40f5df0\"" \
        -DCOMPAT_PROJECT="\"Compat-wireless\"" \
        -DCOMPAT_VERSION="\"compat-wireless-2011-05-19-2-gfa00a5a\""

obj-y += compat.o \
         kstrtox.o \
         compat-2.6.39.o \
         compat-2.6.38.o \
         compat-2.6.37.o \
         kfifo.o \
         compat-2.6.36.o \
         compat-2.6.35.o \
         compat-2.6.33.o \
         compat_firmware_class.o

#else
#obj-m += compat.o
#endif
#compat-objs :=

obj-$(CONFIG_COMPAT_FIRMWARE_CLASS) += compat_firmware_class.o

compat-y += main.o

# Compat kernel compatibility code
compat-$(CONFIG_COMPAT_KERNEL_2_6_14) += compat-2.6.14.o
compat-$(CONFIG_COMPAT_KERNEL_2_6_18) += compat-2.6.18.o
compat-$(CONFIG_COMPAT_KERNEL_2_6_19) += compat-2.6.19.o
compat-$(CONFIG_COMPAT_KERNEL_2_6_21) += compat-2.6.21.o
compat-$(CONFIG_COMPAT_KERNEL_2_6_22) += compat-2.6.22.o
compat-$(CONFIG_COMPAT_KERNEL_2_6_23) += compat-2.6.23.o
compat-$(CONFIG_COMPAT_KERNEL_2_6_24) += compat-2.6.24.o
compat-$(CONFIG_COMPAT_KERNEL_2_6_25) += \
	compat-2.6.25.o \
	pm_qos_params.o

compat-$(CONFIG_COMPAT_KERNEL_2_6_26) += compat-2.6.26.o
compat-$(CONFIG_COMPAT_KERNEL_2_6_27) += compat-2.6.27.o
compat-$(CONFIG_COMPAT_KERNEL_2_6_28) += compat-2.6.28.o
compat-$(CONFIG_COMPAT_KERNEL_2_6_29) += compat-2.6.29.o
compat-$(CONFIG_COMPAT_KERNEL_2_6_32) += compat-2.6.32.o
compat-$(CONFIG_COMPAT_KERNEL_2_6_33) += compat-2.6.33.o
compat-$(CONFIG_COMPAT_KERNEL_2_6_35) += compat-2.6.35.o
compat-$(CONFIG_COMPAT_KERNEL_2_6_36) += \
	compat-2.6.36.o \
	kfifo.o

compat-$(CONFIG_COMPAT_KERNEL_2_6_37) += compat-2.6.37.o
compat-$(CONFIG_COMPAT_KERNEL_2_6_38) += compat-2.6.38.o
compat-$(CONFIG_COMPAT_KERNEL_2_6_39) += \
	compat-2.6.39.o \
	kstrtox.o
