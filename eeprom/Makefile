# This Makefile is generated by the made script:
# https://github.com/alx741/made
#
# Replace FILE with your filename
# Replace MMCU with the target chip model
#
# Dependencies:
# 	avr-gcc
# 	avr-binutils


FILE=test
MMCU=atmega32a

$(FILE).hex: $(FILE).elf
	avr-objcopy -j .text -j .data -O ihex $< $@

$(FILE).elf: $(FILE).c
	avr-gcc -g -Os -mmcu=$(MMCU) $< -o $@

clean:
	rm $(FILE).elf $(FILE).hex
