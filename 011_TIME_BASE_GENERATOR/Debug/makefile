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
010_TIME_BASE_GENERATOR.elf \

SIZE_OUTPUT += \
default.size.stdout \

OBJDUMP_LIST += \
010_TIME_BASE_GENERATOR.list \

OBJCOPY_BIN += \
010_TIME_BASE_GENERATOR.bin \


# All Target
all: 010_TIME_BASE_GENERATOR.elf secondary-outputs

# Tool invocations
010_TIME_BASE_GENERATOR.elf: $(OBJS) $(USER_OBJS) C:\Users\Ronald\ Quino\ Bueno\Desktop\CURSOS\ UDEMY\STM32\CODIGO\ESPACIO\ DEL\ TRABAJO\011_TIME_BASE_GENERATOR\STM32F103C8TX_FLASH.ld
	arm-none-eabi-gcc -o "010_TIME_BASE_GENERATOR.elf" @"objects.list" $(USER_OBJS) $(LIBS) -mcpu=cortex-m3 -T"C:\Users\Ronald Quino Bueno\Desktop\CURSOS UDEMY\STM32\CODIGO\ESPACIO DEL TRABAJO\011_TIME_BASE_GENERATOR\STM32F103C8TX_FLASH.ld" --specs=nosys.specs -Wl,-Map="010_TIME_BASE_GENERATOR.map" -Wl,--gc-sections -static --specs=nano.specs -mfloat-abi=soft -mthumb -Wl,--start-group -lc -lm -Wl,--end-group
	@echo 'Finished building target: $@'
	@echo ' '

default.size.stdout: $(EXECUTABLES)
	arm-none-eabi-size  $(EXECUTABLES)
	@echo 'Finished building: $@'
	@echo ' '

010_TIME_BASE_GENERATOR.list: $(EXECUTABLES)
	arm-none-eabi-objdump -h -S $(EXECUTABLES) > "010_TIME_BASE_GENERATOR.list"
	@echo 'Finished building: $@'
	@echo ' '

010_TIME_BASE_GENERATOR.bin: $(EXECUTABLES)
	arm-none-eabi-objcopy  -O binary $(EXECUTABLES) "010_TIME_BASE_GENERATOR.bin"
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
