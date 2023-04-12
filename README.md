# STM32F4XX_HID_Bootloader

Beware!! Here is a note to keep the bootloader as small as possible
LED PC13 solid means the bootloader is running or empty application

- Empty application will turn the LED PC13 on
  - The program continue to APP memory space
  - because the program is empty it will stuck there ( the LED PC13 on forever)
  
- Pull-down A0 will
  - boot from the bootloader indicated by LED PC13 turn on

if you are using STM32F401CC_bootloader_usbcdc_enabled.bin
  - normal operation will blink the LED PC13 with COM port detected
  - LED PC13 turn on means you are entering the bootloader
