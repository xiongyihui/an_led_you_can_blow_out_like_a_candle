# This file was automagically generated by mbed.org. For more information, 
# see http://mbed.org/handbook/Exporting-to-GCC-ARM-Embedded

###############################################################################
# Boiler-plate

# cross-platform directory manipulation
ifeq ($(shell echo $$OS),$$OS)
    MAKEDIR = if not exist "$(1)" mkdir "$(1)"
    RM = rmdir /S /Q "$(1)"
else
    MAKEDIR = '$(SHELL)' -c "mkdir -p \"$(1)\""
    RM = '$(SHELL)' -c "rm -rf \"$(1)\""
endif

OBJDIR := BUILD
# Move to the build directory
ifeq (,$(filter $(OBJDIR),$(notdir $(CURDIR))))
.SUFFIXES:
mkfile_path := $(abspath $(lastword $(MAKEFILE_LIST)))
MAKETARGET = '$(MAKE)' --no-print-directory -C $(OBJDIR) -f '$(mkfile_path)' \
		'SRCDIR=$(CURDIR)' $(MAKECMDGOALS)
.PHONY: $(OBJDIR) clean
all:
	+@$(call MAKEDIR,$(OBJDIR))
	+@$(MAKETARGET)
$(OBJDIR): all
Makefile : ;
% :: $(OBJDIR) ; :
clean :
	$(call RM,$(OBJDIR))

else

# trick rules into thinking we are in the root, when we are in the bulid dir
VPATH = ..

# Boiler-plate
###############################################################################
# Project settings

PROJECT := led_like_a_candle


# Project settings
###############################################################################
# Objects and Paths

OBJECTS += BufferedSerial/Buffer/Buffer.o
OBJECTS += BufferedSerial/BufferedSerial.o
OBJECTS += USBDevice/USBAudio/USBAudio.o
OBJECTS += USBDevice/USBDevice/USBDevice.o
OBJECTS += USBDevice/USBDevice/USBHAL_EFM32.o
OBJECTS += USBDevice/USBDevice/USBHAL_KL25Z.o
OBJECTS += USBDevice/USBDevice/USBHAL_LPC11U.o
OBJECTS += USBDevice/USBDevice/USBHAL_LPC17.o
OBJECTS += USBDevice/USBDevice/USBHAL_LPC40.o
OBJECTS += USBDevice/USBDevice/USBHAL_Maxim.o
OBJECTS += USBDevice/USBDevice/USBHAL_RZ_A1H.o
OBJECTS += USBDevice/USBDevice/USBHAL_STM32F4.o
OBJECTS += USBDevice/USBHID/USBHID.o
OBJECTS += USBDevice/USBHID/USBKeyboard.o
OBJECTS += USBDevice/USBHID/USBMouse.o
OBJECTS += USBDevice/USBHID/USBMouseKeyboard.o
OBJECTS += USBDevice/USBMIDI/USBMIDI.o
OBJECTS += USBDevice/USBMSD/USBMSD.o
OBJECTS += USBDevice/USBSerial/USBCDC.o
OBJECTS += USBDevice/USBSerial/USBSerial.o
OBJECTS += main.o

 SYS_OBJECTS += mbed/TARGET_ARCH_PRO/TOOLCHAIN_GCC_ARM/board.o
 SYS_OBJECTS += mbed/TARGET_ARCH_PRO/TOOLCHAIN_GCC_ARM/cmsis_nvic.o
 SYS_OBJECTS += mbed/TARGET_ARCH_PRO/TOOLCHAIN_GCC_ARM/retarget.o
 SYS_OBJECTS += mbed/TARGET_ARCH_PRO/TOOLCHAIN_GCC_ARM/startup_LPC17xx.o
 SYS_OBJECTS += mbed/TARGET_ARCH_PRO/TOOLCHAIN_GCC_ARM/system_LPC17xx.o

INCLUDE_PATHS += -I../.
INCLUDE_PATHS += -I../BufferedSerial
INCLUDE_PATHS += -I../BufferedSerial/Buffer
INCLUDE_PATHS += -I../USBDevice
INCLUDE_PATHS += -I../USBDevice/USBAudio
INCLUDE_PATHS += -I../USBDevice/USBDevice
INCLUDE_PATHS += -I../USBDevice/USBHID
INCLUDE_PATHS += -I../USBDevice/USBMIDI
INCLUDE_PATHS += -I../USBDevice/USBMSD
INCLUDE_PATHS += -I../USBDevice/USBSerial
INCLUDE_PATHS += -I../mbed
INCLUDE_PATHS += -I../mbed/TARGET_ARCH_PRO
INCLUDE_PATHS += -I../mbed/TARGET_ARCH_PRO/TARGET_NXP/TARGET_LPC176X
INCLUDE_PATHS += -I../mbed/TARGET_ARCH_PRO/TARGET_NXP/TARGET_LPC176X/TARGET_ARCH_PRO

LIBRARY_PATHS := -L../mbed/TARGET_ARCH_PRO/TOOLCHAIN_GCC_ARM 
LIBRARIES := -lmbed 
LINKER_SCRIPT ?= ../mbed/TARGET_ARCH_PRO/TOOLCHAIN_GCC_ARM/LPC1768.ld

# Objects and Paths
###############################################################################
# Tools and Flags

AS      = arm-none-eabi-gcc
CC      = arm-none-eabi-gcc
CPP     = arm-none-eabi-g++
LD      = arm-none-eabi-gcc
ELF2BIN = arm-none-eabi-objcopy
PREPROC = arm-none-eabi-cpp -E -P -Wl,--gc-sections -Wl,--wrap,main -mcpu=cortex-m3 -mthumb


C_FLAGS += -std=gnu99
C_FLAGS += -include
C_FLAGS += mbed_config.h
C_FLAGS += -DDEVICE_EMAC=1
C_FLAGS += -D__MBED__=1
C_FLAGS += -DMBED_BUILD_TIMESTAMP=1545988169.84
C_FLAGS += -DTARGET_LIKE_MBED
C_FLAGS += -DTARGET_NXP
C_FLAGS += -DTARGET_ARCH_PRO
C_FLAGS += -D__MBED_CMSIS_RTOS_CM
C_FLAGS += -D__CMSIS_RTOS
C_FLAGS += -DTARGET_FF_ARDUINO
C_FLAGS += -DTOOLCHAIN_GCC
C_FLAGS += -DDEVICE_CAN=1
C_FLAGS += -DTARGET_LIKE_CORTEX_M3
C_FLAGS += -DTARGET_CORTEX_M
C_FLAGS += -DARM_MATH_CM3
C_FLAGS += -DDEVICE_ANALOGOUT=1
C_FLAGS += -DTARGET_LPC176X
C_FLAGS += -DTARGET_NXP_EMAC
C_FLAGS += -DTARGET_M3
C_FLAGS += -DDEVICE_SERIAL=1
C_FLAGS += -DDEVICE_INTERRUPTIN=1
C_FLAGS += -DTARGET_LPCTarget
C_FLAGS += -DTARGET_CORTEX
C_FLAGS += -DDEVICE_I2C=1
C_FLAGS += -DDEVICE_PORTOUT=1
C_FLAGS += -D__CORTEX_M3
C_FLAGS += -DDEVICE_STDIO_MESSAGES=1
C_FLAGS += -DTARGET_LPC1768
C_FLAGS += -DTARGET_RELEASE
C_FLAGS += -DDEVICE_SERIAL_FC=1
C_FLAGS += -DDEVICE_PORTINOUT=1
C_FLAGS += -DDEVICE_I2CSLAVE=1
C_FLAGS += -DDEVICE_PORTIN=1
C_FLAGS += -DDEVICE_SLEEP=1
C_FLAGS += -DTOOLCHAIN_GCC_ARM
C_FLAGS += -DDEVICE_SPI=1
C_FLAGS += -DDEVICE_ETHERNET=1
C_FLAGS += -DDEVICE_SPISLAVE=1
C_FLAGS += -DDEVICE_ANALOGIN=1
C_FLAGS += -DDEVICE_PWMOUT=1
C_FLAGS += -DDEVICE_FLASH=1
C_FLAGS += -DDEVICE_DEBUG_AWARENESS=1
C_FLAGS += -include
C_FLAGS += mbed_config.h
C_FLAGS += -std=gnu99
C_FLAGS += -c
C_FLAGS += -Wall
C_FLAGS += -Wextra
C_FLAGS += -Wno-unused-parameter
C_FLAGS += -Wno-missing-field-initializers
C_FLAGS += -fmessage-length=0
C_FLAGS += -fno-exceptions
C_FLAGS += -fno-builtin
C_FLAGS += -ffunction-sections
C_FLAGS += -fdata-sections
C_FLAGS += -funsigned-char
C_FLAGS += -MMD
C_FLAGS += -fno-delete-null-pointer-checks
C_FLAGS += -fomit-frame-pointer
C_FLAGS += -Os
C_FLAGS += -g1
C_FLAGS += -mcpu=cortex-m3
C_FLAGS += -mthumb
C_FLAGS += -DMBED_ROM_START=0x0
C_FLAGS += -DMBED_ROM_SIZE=0x80000

CXX_FLAGS += -std=gnu++98
CXX_FLAGS += -fno-rtti
CXX_FLAGS += -Wvla
CXX_FLAGS += -include
CXX_FLAGS += mbed_config.h
CXX_FLAGS += -DDEVICE_EMAC=1
CXX_FLAGS += -D__MBED__=1
CXX_FLAGS += -DMBED_BUILD_TIMESTAMP=1545988169.84
CXX_FLAGS += -DTARGET_LIKE_MBED
CXX_FLAGS += -DTARGET_NXP
CXX_FLAGS += -DTARGET_ARCH_PRO
CXX_FLAGS += -D__MBED_CMSIS_RTOS_CM
CXX_FLAGS += -D__CMSIS_RTOS
CXX_FLAGS += -DTARGET_FF_ARDUINO
CXX_FLAGS += -DTOOLCHAIN_GCC
CXX_FLAGS += -DDEVICE_CAN=1
CXX_FLAGS += -DTARGET_LIKE_CORTEX_M3
CXX_FLAGS += -DTARGET_CORTEX_M
CXX_FLAGS += -DARM_MATH_CM3
CXX_FLAGS += -DDEVICE_ANALOGOUT=1
CXX_FLAGS += -DTARGET_LPC176X
CXX_FLAGS += -DTARGET_NXP_EMAC
CXX_FLAGS += -DTARGET_M3
CXX_FLAGS += -DDEVICE_SERIAL=1
CXX_FLAGS += -DDEVICE_INTERRUPTIN=1
CXX_FLAGS += -DTARGET_LPCTarget
CXX_FLAGS += -DTARGET_CORTEX
CXX_FLAGS += -DDEVICE_I2C=1
CXX_FLAGS += -DDEVICE_PORTOUT=1
CXX_FLAGS += -D__CORTEX_M3
CXX_FLAGS += -DDEVICE_STDIO_MESSAGES=1
CXX_FLAGS += -DTARGET_LPC1768
CXX_FLAGS += -DTARGET_RELEASE
CXX_FLAGS += -DDEVICE_SERIAL_FC=1
CXX_FLAGS += -DDEVICE_PORTINOUT=1
CXX_FLAGS += -DDEVICE_I2CSLAVE=1
CXX_FLAGS += -DDEVICE_PORTIN=1
CXX_FLAGS += -DDEVICE_SLEEP=1
CXX_FLAGS += -DTOOLCHAIN_GCC_ARM
CXX_FLAGS += -DDEVICE_SPI=1
CXX_FLAGS += -DDEVICE_ETHERNET=1
CXX_FLAGS += -DDEVICE_SPISLAVE=1
CXX_FLAGS += -DDEVICE_ANALOGIN=1
CXX_FLAGS += -DDEVICE_PWMOUT=1
CXX_FLAGS += -DDEVICE_FLASH=1
CXX_FLAGS += -DDEVICE_DEBUG_AWARENESS=1
CXX_FLAGS += -include
CXX_FLAGS += mbed_config.h
CXX_FLAGS += -std=gnu++98
CXX_FLAGS += -fno-rtti
CXX_FLAGS += -Wvla
CXX_FLAGS += -c
CXX_FLAGS += -Wall
CXX_FLAGS += -Wextra
CXX_FLAGS += -Wno-unused-parameter
CXX_FLAGS += -Wno-missing-field-initializers
CXX_FLAGS += -fmessage-length=0
CXX_FLAGS += -fno-exceptions
CXX_FLAGS += -fno-builtin
CXX_FLAGS += -ffunction-sections
CXX_FLAGS += -fdata-sections
CXX_FLAGS += -funsigned-char
CXX_FLAGS += -MMD
CXX_FLAGS += -fno-delete-null-pointer-checks
CXX_FLAGS += -fomit-frame-pointer
CXX_FLAGS += -Os
CXX_FLAGS += -g1
CXX_FLAGS += -mcpu=cortex-m3
CXX_FLAGS += -mthumb
CXX_FLAGS += -DMBED_ROM_START=0x0
CXX_FLAGS += -DMBED_ROM_SIZE=0x80000

ASM_FLAGS += -x
ASM_FLAGS += assembler-with-cpp
ASM_FLAGS += -D__CMSIS_RTOS
ASM_FLAGS += -D__MBED_CMSIS_RTOS_CM
ASM_FLAGS += -D__CORTEX_M3
ASM_FLAGS += -DARM_MATH_CM3
ASM_FLAGS += -DTARGET_LPC1768
ASM_FLAGS += -I../.
ASM_FLAGS += -I../BufferedSerial
ASM_FLAGS += -I../BufferedSerial/Buffer
ASM_FLAGS += -I../USBDevice
ASM_FLAGS += -I../USBDevice/USBAudio
ASM_FLAGS += -I../USBDevice/USBDevice
ASM_FLAGS += -I../USBDevice/USBHID
ASM_FLAGS += -I../USBDevice/USBMIDI
ASM_FLAGS += -I../USBDevice/USBMSD
ASM_FLAGS += -I../USBDevice/USBSerial
ASM_FLAGS += -I../mbed
ASM_FLAGS += -I../mbed/TARGET_ARCH_PRO
ASM_FLAGS += -I../mbed/TARGET_ARCH_PRO/TARGET_NXP/TARGET_LPC176X
ASM_FLAGS += -I../mbed/TARGET_ARCH_PRO/TARGET_NXP/TARGET_LPC176X/TARGET_ARCH_PRO
ASM_FLAGS += -include
ASM_FLAGS += /filer/workspace_data/exports/0/05b93868eeeb6058ba08b50a100e2f8d/USB2UART_origin/mbed_config.h
ASM_FLAGS += -x
ASM_FLAGS += assembler-with-cpp
ASM_FLAGS += -c
ASM_FLAGS += -Wall
ASM_FLAGS += -Wextra
ASM_FLAGS += -Wno-unused-parameter
ASM_FLAGS += -Wno-missing-field-initializers
ASM_FLAGS += -fmessage-length=0
ASM_FLAGS += -fno-exceptions
ASM_FLAGS += -fno-builtin
ASM_FLAGS += -ffunction-sections
ASM_FLAGS += -fdata-sections
ASM_FLAGS += -funsigned-char
ASM_FLAGS += -MMD
ASM_FLAGS += -fno-delete-null-pointer-checks
ASM_FLAGS += -fomit-frame-pointer
ASM_FLAGS += -Os
ASM_FLAGS += -g1
ASM_FLAGS += -mcpu=cortex-m3
ASM_FLAGS += -mthumb


LD_FLAGS :=-Wl,--gc-sections -Wl,--wrap,main -mcpu=cortex-m3 -mthumb 
LD_SYS_LIBS :=-Wl,--start-group -lstdc++ -lsupc++ -lm -lc -lgcc -lnosys -lmbed -Wl,--end-group

# Tools and Flags
###############################################################################
# Rules

.PHONY: all lst size


all: $(PROJECT).bin $(PROJECT).hex size


.s.o:
	+@$(call MAKEDIR,$(dir $@))
	+@echo "Assemble: $(notdir $<)"
  
	@$(AS) -c $(ASM_FLAGS) -o $@ $<
  


.S.o:
	+@$(call MAKEDIR,$(dir $@))
	+@echo "Assemble: $(notdir $<)"
  
	@$(AS) -c $(ASM_FLAGS) -o $@ $<
  

.c.o:
	+@$(call MAKEDIR,$(dir $@))
	+@echo "Compile: $(notdir $<)"
	@$(CC) $(C_FLAGS) $(INCLUDE_PATHS) -o $@ $<

.cpp.o:
	+@$(call MAKEDIR,$(dir $@))
	+@echo "Compile: $(notdir $<)"
	@$(CPP) $(CXX_FLAGS) $(INCLUDE_PATHS) -o $@ $<


$(PROJECT).link_script.ld: $(LINKER_SCRIPT)
	@$(PREPROC) $< -o $@



$(PROJECT).elf: $(OBJECTS) $(SYS_OBJECTS) $(PROJECT).link_script.ld 
	+@echo "link: $(notdir $@)"
	@$(LD) $(LD_FLAGS) -T $(filter-out %.o, $^) $(LIBRARY_PATHS) --output $@ $(filter %.o, $^) $(LIBRARIES) $(LD_SYS_LIBS)


$(PROJECT).bin: $(PROJECT).elf
	$(ELF2BIN) -O binary $< $@
	+@echo "===== bin file ready to flash: $(OBJDIR)/$@ =====" 

$(PROJECT).hex: $(PROJECT).elf
	$(ELF2BIN) -O ihex $< $@


# Rules
###############################################################################
# Dependencies

DEPS = $(OBJECTS:.o=.d) $(SYS_OBJECTS:.o=.d)
-include $(DEPS)
endif

# Dependencies
###############################################################################
