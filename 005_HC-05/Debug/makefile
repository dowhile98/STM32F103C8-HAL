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
005_HC-05.elf \

SIZE_OUTPUT += \
default.size.stdout \

OBJDUMP_LIST += \
005_HC-05.list \


# All Target
all: 005_HC-05.elf secondary-outputs

# Tool invocations
005_HC-05.elf: $(OBJS) $(USER_OBJS) F:\CURSOS\ UDEMY\STM32\MCU2\CODIGO\ESPACIO\ DE\ TRABAJO\005_HC-05\STM32F103C8TX_FLASH.ld
	arm-none-eabi-gcc -o "005_HC-05.elf" @"objects.list" $(USER_OBJS) $(LIBS) -mcpu=cortex-m3 -T"F:\CURSOS UDEMY\STM32\MCU2\CODIGO\ESPACIO DE TRABAJO\005_HC-05\STM32F103C8TX_FLASH.ld" --specs=nosys.specs -Wl,-Map="005_HC-05.map" -Wl,--gc-sections -static --specs=nano.specs -mfloat-abi=soft -mthumb -Wl,--start-group -lc -lm -Wl,--end-group
	@echo 'Finished building target: $@'
	@echo ' '

default.size.stdout: $(EXECUTABLES)
	arm-none-eabi-size  $(EXECUTABLES)
	@echo 'Finished building: $@'
	@echo ' '

005_HC-05.list: $(EXECUTABLES)
	arm-none-eabi-objdump -h -S $(EXECUTABLES) > "005_HC-05.list"
	@echo 'Finished building: $@'
	@echo ' '

# Other Targets
clean:
	-$(RM) *
	-@echo ' '

secondary-outputs: $(SIZE_OUTPUT) $(OBJDUMP_LIST)

.PHONY: all clean dependents
.SECONDARY:

-include ../makefile.targets
