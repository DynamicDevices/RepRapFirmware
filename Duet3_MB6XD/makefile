################################################################################
# Automatically-generated file. Do not edit!
################################################################################

-include ../makefile.init

RM := rm -rf

# All of the sources participating in the build are defined here
-include sources.mk
-include src/libcpp/subdir.mk
-include src/libc/subdir.mk
-include src/bossa/subdir.mk
-include src/Tools/subdir.mk
-include src/Storage/subdir.mk
-include src/SBC/subdir.mk
-include src/PrintMonitor/subdir.mk
-include src/Platform/subdir.mk
-include src/ObjectModel/subdir.mk
-include src/Networking/MulticastDiscovery/subdir.mk
-include src/Networking/MQTT/MQTT_C/src/subdir.mk
-include src/Networking/MQTT/subdir.mk
-include src/Networking/LwipEthernet/Lwip/src/netif/subdir.mk
-include src/Networking/LwipEthernet/Lwip/src/core/ipv6/subdir.mk
-include src/Networking/LwipEthernet/Lwip/src/core/ipv4/subdir.mk
-include src/Networking/LwipEthernet/Lwip/src/core/subdir.mk
-include src/Networking/LwipEthernet/Lwip/src/apps/netbiosns/subdir.mk
-include src/Networking/LwipEthernet/Lwip/src/apps/mdns/subdir.mk
-include src/Networking/LwipEthernet/Lwip/src/api/subdir.mk
-include src/Networking/LwipEthernet/GMAC/subdir.mk
-include src/Networking/LwipEthernet/subdir.mk
-include src/Networking/subdir.mk
-include src/Movement/StepperDrivers/subdir.mk
-include src/Movement/Kinematics/subdir.mk
-include src/Movement/HeightControl/subdir.mk
-include src/Movement/BedProbing/subdir.mk
-include src/Movement/subdir.mk
-include src/Libraries/sha1/subdir.mk
-include src/Libraries/sd_mmc/subdir.mk
-include src/Libraries/Fatfs/subdir.mk
-include src/LedStrips/subdir.mk
-include src/InputMonitors/subdir.mk
-include src/Heating/Sensors/subdir.mk
-include src/Heating/subdir.mk
-include src/Hardware/Spi/subdir.mk
-include src/Hardware/SAME70/Ethernet/ksz8081rna/subdir.mk
-include src/Hardware/SAME70/Ethernet/subdir.mk
-include src/Hardware/SAME70/subdir.mk
-include src/Hardware/subdir.mk
-include src/GPIO/subdir.mk
-include src/GCodes/GCodeBuffer/subdir.mk
-include src/GCodes/subdir.mk
-include src/FilamentMonitors/subdir.mk
-include src/Fans/subdir.mk
-include src/Endstops/subdir.mk
-include src/Config/subdir.mk
-include src/Comms/subdir.mk
-include src/ClosedLoop/subdir.mk
-include src/CAN/subdir.mk
-include src/Accelerometers/subdir.mk
-include src/subdir.mk
ifneq ($(MAKECMDGOALS),clean)
ifneq ($(strip $(C++M_DEPS)),)
-include $(C++M_DEPS)
endif
ifneq ($(strip $(C++_DEPS)),)
-include $(C++_DEPS)
endif
ifneq ($(strip $(CCM_DEPS)),)
-include $(CCM_DEPS)
endif
ifneq ($(strip $(CC_DEPS)),)
-include $(CC_DEPS)
endif
ifneq ($(strip $(CPP_DEPS)),)
-include $(CPP_DEPS)
endif
ifneq ($(strip $(CXXM_DEPS)),)
-include $(CXXM_DEPS)
endif
ifneq ($(strip $(CXX_DEPS)),)
-include $(CXX_DEPS)
endif
ifneq ($(strip $(C_DEPS)),)
-include $(C_DEPS)
endif
ifneq ($(strip $(C_UPPER_DEPS)),)
-include $(C_UPPER_DEPS)
endif
endif

-include ../makefile.defs

OPTIONAL_TOOL_DEPS := \
$(wildcard ../makefile.defs) \
$(wildcard ../makefile.init) \
$(wildcard ../makefile.targets) \


BUILD_ARTIFACT_NAME := Duet3Firmware_MB6XD
BUILD_ARTIFACT_EXTENSION := elf
BUILD_ARTIFACT_PREFIX :=
BUILD_ARTIFACT := $(BUILD_ARTIFACT_PREFIX)$(BUILD_ARTIFACT_NAME)$(if $(BUILD_ARTIFACT_EXTENSION),.$(BUILD_ARTIFACT_EXTENSION),)

# Add inputs and outputs from these tool invocations to the build variables 

# All Target
all:
	+@$(MAKE) --no-print-directory main-build && $(MAKE) --no-print-directory post-build

# Main-build Target
main-build: Duet3Firmware_MB6XD.elf

dependents:
	-cd /home/ajlennon/git/RepRapFirmware-Builder/CANLib/SAME70_RTOS && $(MAKE) all
	-cd /home/ajlennon/git/RepRapFirmware-Builder/FreeRTOS/SAME70 && $(MAKE) all
	-cd /home/ajlennon/git/RepRapFirmware-Builder/RRFLibraries/SAME70_RTOS && $(MAKE) all
	-cd /home/ajlennon/git/RepRapFirmware-Builder/CoreN2G/SAME70_CAN_SDHC_USB_RTOS && $(MAKE) all

# Tool invocations
Duet3Firmware_MB6XD.elf: $(OBJS) $(USER_OBJS) /home/ajlennon/git/RepRapFirmware-Builder/CANLib/SAME70_RTOS/libCANlib.a /home/ajlennon/git/RepRapFirmware-Builder/FreeRTOS/SAME70/libFreeRTOS.a /home/ajlennon/git/RepRapFirmware-Builder/RRFLibraries/SAME70_RTOS/libRRFLibraries.a /home/ajlennon/git/RepRapFirmware-Builder/CoreN2G/SAME70_CAN_SDHC_USB_RTOS/libCoreN2G.a makefile $(OPTIONAL_TOOL_DEPS)
	@echo 'Building target: $@'
	@echo 'Invoking: Cross G++ Linker'
	arm-none-eabi-gcc -L"/home/ajlennon/git/RepRapFirmware-Builder/CoreN2G/SAME70_CAN_SDHC_USB_RTOS" -L"/home/ajlennon/git/RepRapFirmware-Builder/RRFLibraries/SAME70_RTOS" -L"/home/ajlennon/git/RepRapFirmware-Builder/FreeRTOS/SAME70" -L"/home/ajlennon/git/RepRapFirmware-Builder/CANLib/SAME70_RTOS" --specs=nosys.specs -Os -Wl,--gc-sections -Wl,--fatal-warnings -Wl,--no-warn-rwx-segment -mcpu=cortex-m7 -mfpu=fpv5-d16 -mfloat-abi=hard -T"/home/ajlennon/git/RepRapFirmware-Builder/RepRapFirmware/src/Hardware/SAME70/same70q20b_flash.ld" -Wl,-Map,"/home/ajlennon/git/RepRapFirmware-Builder/RepRapFirmware/Duet3_MB6XD/Duet3Firmware_MB6XD.map" -o "Duet3Firmware_MB6XD.elf" -mthumb -Wl,--cref -Wl,--check-sections -Wl,--gc-sections -Wl,--entry=Reset_Handler -Wl,--unresolved-symbols=report-all -Wl,--warn-common -Wl,--warn-section-align -Wl,--warn-unresolved-symbols -Wl,--start-group $(OBJS) $(USER_OBJS) $(LIBS) -lCoreN2G -lRRFLibraries -lFreeRTOS -lCANlib -lsupc++ -Wl,--end-group -lm
	@echo 'Finished building target: $@'
	@echo ' '

# Other Targets
clean:
	-$(RM) Duet3Firmware_MB6XD.elf
	-@echo ' '

post-build:
	-@echo 'Generating binary file'
	-arm-none-eabi-objcopy -O binary "/home/ajlennon/git/RepRapFirmware-Builder/RepRapFirmware/Duet3_MB6XD/Duet3Firmware_MB6XD.elf" "/home/ajlennon/git/RepRapFirmware-Builder/RepRapFirmware/Duet3_MB6XD/Duet3Firmware_MB6XD.bin" && CrcAppender "/home/ajlennon/git/RepRapFirmware-Builder/RepRapFirmware/Duet3_MB6XD/Duet3Firmware_MB6XD.bin"
	-@echo ' '

.PHONY: all clean dependents main-build post-build
/home/ajlennon/git/RepRapFirmware-Builder/CANLib/SAME70_RTOS/libCANlib.a:
/home/ajlennon/git/RepRapFirmware-Builder/FreeRTOS/SAME70/libFreeRTOS.a:
/home/ajlennon/git/RepRapFirmware-Builder/RRFLibraries/SAME70_RTOS/libRRFLibraries.a:
/home/ajlennon/git/RepRapFirmware-Builder/CoreN2G/SAME70_CAN_SDHC_USB_RTOS/libCoreN2G.a:

-include ../makefile.targets
