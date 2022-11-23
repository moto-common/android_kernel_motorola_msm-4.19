obj-$(CONFIG_TOUCHSCREEN_ILITEK_CHIPSET) += ilitek_0flash_mmi.o

ifneq ($(filter m y,$(CONFIG_INPUT_ILI_0FLASH_MMI_ENABLE_DOUBLE_TAP)),)
	EXTRA_CFLAGS += -DILI_SENSOR_EN
endif
ifneq ($(filter m y,$(CONFIG_INPUT_ILI_PANEL_NOTIFICATIONS)),)
	EXTRA_CFLAGS += -DILI_CONFIG_PANEL_NOTIFICATIONS
endif
ifneq ($(filter m y,$(CONFIG_ILITEK_RESUME_BY_DDI)),)
	EXTRA_CFLAGS += -DILI_CONFIG_RESUME_BY_DDI
endif

ilitek_0flash_mmi-objs += ilitek.o
ilitek_0flash_mmi-objs += ilitek_spi.o
ilitek_0flash_mmi-objs += ilitek_qcom.o
ilitek_0flash_mmi-objs += ilitek_ic.o
ilitek_0flash_mmi-objs += ilitek_touch.o
ilitek_0flash_mmi-objs += ilitek_mp.o
ilitek_0flash_mmi-objs += ilitek_hostdl.o
ilitek_0flash_mmi-objs += ilitek_node.o
