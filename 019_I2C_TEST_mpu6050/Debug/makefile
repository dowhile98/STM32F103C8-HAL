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
019_I2C_TEST_mpu6050.elf \

SIZE_OUTPUT += \
default.size.stdout \

OBJDUMP_LIST += \
019_I2C_TEST_mpu6050.list \

OBJCOPY_BIN += \
019_I2C_TEST_mpu6050.bin \


# All Target
all: 019_I2C_TEST_mpu6050.elf secondary-outputs

# Tool invocations
019_I2C_TEST_mpu6050.elf: $(OBJS) $(USER_OBJS) C:\Users\Ronald\ Quino\ Bueno\Desktop\CURSOS\ UDEMY\STM32\CODIGO\ESPACIO\ DEL\ TRABAJO\019_I2C_TEST_mpu6050\STM32F103C8TX_FLASH.ld
	arm-none-eabi-gcc -o "019_I2C_TEST_mpu6050.elf" @"objects.list" $(USER_OBJS) $(LIBS) -mcpu=cortex-m3 -T"C:\Users\Ronald Quino Bueno\Desktop\CURSOS UDEMY\STM32\CODIGO\ESPACIO DEL TRABAJO\019_I2C_TEST_mpu6050\STM32F103C8TX_FLASH.ld" --specs=nosys.specs -Wl,-Map="019_I2C_TEST_mpu6050.map" -Wl,--gc-sections -static -u_printf_float --specs=nano.specs -mfloat-abi=soft -mthumb -Wl,--start-group -lc -lm -Wl,--end-group
	@echo 'Finished building target: $@'
	@echo ' '

default.size.stdout: $(EXECUTABLES)
	arm-none-eabi-size  $(EXECUTABLES)
	@echo 'Finished building: $@'
	@echo ' '

019_I2C_TEST_mpu6050.list: $(EXECUTABLES)
	arm-none-eabi-objdump -h -S $(EXECUTABLES) > "019_I2C_TEST_mpu6050.list"
	@echo 'Finished building: $@'
	@echo ' '

019_I2C_TEST_mpu6050.bin: $(EXECUTABLES)
	arm-none-eabi-objcopy  -O binary $(EXECUTABLES) "019_I2C_TEST_mpu6050.bin"
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
