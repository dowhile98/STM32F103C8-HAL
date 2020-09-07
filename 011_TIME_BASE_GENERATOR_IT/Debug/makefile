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
011_TIME_BASE_GENERATOR_IT.elf \

SIZE_OUTPUT += \
default.size.stdout \

OBJDUMP_LIST += \
011_TIME_BASE_GENERATOR_IT.list \

OBJCOPY_BIN += \
011_TIME_BASE_GENERATOR_IT.bin \


# All Target
all: 011_TIME_BASE_GENERATOR_IT.elf secondary-outputs

# Tool invocations
011_TIME_BASE_GENERATOR_IT.elf: $(OBJS) $(USER_OBJS) C:\Users\Ronald\ Quino\ Bueno\Desktop\CURSOS\ UDEMY\STM32\CODIGO\ESPACIO\ DEL\ TRABAJO\011_TIME_BASE_GENERATOR_IT\STM32F103C8TX_FLASH.ld
	arm-none-eabi-gcc -o "011_TIME_BASE_GENERATOR_IT.elf" @"objects.list" $(USER_OBJS) $(LIBS) -mcpu=cortex-m3 -T"C:\Users\Ronald Quino Bueno\Desktop\CURSOS UDEMY\STM32\CODIGO\ESPACIO DEL TRABAJO\011_TIME_BASE_GENERATOR_IT\STM32F103C8TX_FLASH.ld" --specs=nosys.specs -Wl,-Map="011_TIME_BASE_GENERATOR_IT.map" -Wl,--gc-sections -static --specs=nano.specs -mfloat-abi=soft -mthumb -Wl,--start-group -lc -lm -Wl,--end-group
	@echo 'Finished building target: $@'
	@echo ' '

default.size.stdout: $(EXECUTABLES)
	arm-none-eabi-size  $(EXECUTABLES)
	@echo 'Finished building: $@'
	@echo ' '

011_TIME_BASE_GENERATOR_IT.list: $(EXECUTABLES)
	arm-none-eabi-objdump -h -S $(EXECUTABLES) > "011_TIME_BASE_GENERATOR_IT.list"
	@echo 'Finished building: $@'
	@echo ' '

011_TIME_BASE_GENERATOR_IT.bin: $(EXECUTABLES)
	arm-none-eabi-objcopy  -O binary $(EXECUTABLES) "011_TIME_BASE_GENERATOR_IT.bin"
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
