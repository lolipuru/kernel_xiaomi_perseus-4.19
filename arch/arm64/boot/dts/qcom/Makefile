# SPDX-License-Identifier: GPL-2.0
ifeq ($(CONFIG_BUILD_ARM64_DT_OVERLAY),y)
dtbo-$(CONFIG_MACH_XIAOMI_E5) += \
	xiaomi/perseus/perseus-mp-v2.1.dtbo

ifeq ($(CONFIG_MACH_XIAOMI_E5),y)
xiaomi/perseus/perseus-mp-v2.1.dtbo-base := ../sdm845-mtp.dtb
endif

else
dtb-$(CONFIG_ARCH_QCOM)	+= apq8016-sbc.dtb
dtb-$(CONFIG_ARCH_QCOM)	+= apq8096-db820c.dtb
dtb-$(CONFIG_ARCH_QCOM)	+= ipq8074-hk01.dtb
dtb-$(CONFIG_ARCH_QCOM)	+= msm8916-mtp.dtb
dtb-$(CONFIG_ARCH_QCOM)	+= msm8992-bullhead-rev-101.dtb
dtb-$(CONFIG_ARCH_QCOM)	+= msm8994-angler-rev-101.dtb
dtb-$(CONFIG_ARCH_QCOM)	+= msm8996-mtp.dtb
dtb-$(CONFIG_ARCH_QCOM)	+= sdm845-mtp.dtb

dtb-$(CONFIG_MACH_XIAOMI_E10) := xiaomi/beryllium/beryllium-mp-v2.1.dtb
dtb-$(CONFIG_MACH_XIAOMI_E5) := xiaomi/perseus/perseus-mp-v2.1.dtb
endif

always		:= $(dtb-y)
subdir-y	:= $(dts-dirs)
clean-files    := *.dtb *.dtbo
