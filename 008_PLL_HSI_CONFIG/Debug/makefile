################################################################################
# Automatically-generated file. Do not edit!
################################################################################

-include ../makefile.init

RM := rm -rf

# All of the sources participating in the build are defined here
-include sources.mk
-include Drivers/STM32F1xx_HAL_Driver/Src/subdir.mk
-include Core/Startup/subdir.mk
-include Core/Src/subdir.mk
-include subdir.mk
-include objects.mk

ifneq ($(MAKECMDGOALS),clean)
ifneq ($(strip $(C_DEPS)),)
-include $(C_DEPS)
endif
endif

-include ../makefile.defs

# Add inputs and outputs from these tool invocations to the build variables 
EXECUTABLES += \
008_PLL_HSI_CONFIG.elf \

SIZE_OUTPUT += \
default.size.stdout \

OBJDUMP_LIST += \
008_PLL_HSI_CONFIG.list \

OBJCOPY_BIN += \
008_PLL_HSI_CONFIG.bin \


# All Target
all: 008_PLL_HSI_CONFIG.elf secondary-outputs

# Tool invocations
008_PLL_HSI_CONFIG.elf: $(OBJS) $(USER_OBJS) C:\Users\Ronald\ Quino\ Bueno\Dropbox\Mi\ PC\ (LAPTOP-RJV92R15)\Desktop\CURSOS\ UDEMY\STM32\MCU2\CODIGO\STM32F1\008_PLL_HSI_CONFIG\STM32F103C8TX_FLASH.ld
	arm-none-eabi-gcc -o "008_PLL_HSI_CONFIG.elf" @"objects.list" $(USER_OBJS) $(LIBS) -mcpu=cortex-m3 -T"C:\Users\Ronald Quino Bueno\Dropbox\Mi PC (LAPTOP-RJV92R15)\Desktop\CURSOS UDEMY\STM32\MCU2\CODIGO\STM32F1\008_PLL_HSI_CONFIG\STM32F103C8TX_FLASH.ld" --specs=nosys.specs -Wl,-Map="008_PLL_HSI_CONFIG.map" -Wl,--gc-sections -static --specs=nano.specs -mfloat-abi=soft -mthumb -Wl,--start-group -lc -lm -Wl,--end-group
	@echo 'Finished building target: $@'
	@echo ' '

default.size.stdout: $(EXECUTABLES)
	arm-none-eabi-size  $(EXECUTABLES)
	@echo 'Finished building: $@'
	@echo ' '

008_PLL_HSI_CONFIG.list: $(EXECUTABLES)
	arm-none-eabi-objdump -h -S $(EXECUTABLES) > "008_PLL_HSI_CONFIG.list"
	@echo 'Finished building: $@'
	@echo ' '

008_PLL_HSI_CONFIG.bin: $(EXECUTABLES)
	arm-none-eabi-objcopy  -O binary $(EXECUTABLES) "008_PLL_HSI_CONFIG.bin"
	@echo 'Finished building: $@'
	@echo ' '

# Other Targets
clean:
	-$(RM) *
	-@echo ' '

secondary-outputs: $(SIZE_OUTPUT) $(OBJDUMP_LIST) $(OBJCOPY_BIN)

.PHONY: all clean dependents
.SECONDARY:

-include ../makefile.targets
