.. see the [Wiki for firmware](https://github.com/yo8aiv/WIFI-LoRa-32-V2-charging-mod---meshtastic-legacy-firmware-HELTEC-V2.1-/wiki)  and  [GPS mod](https://github.com/yo8aiv/WIFI-LoRa-32-V2-charging-and-gps-mod-meshtastic-legacy-firmware-HELTEC-V2.1/wiki/Heltec-V2-,-Heltec-V2.1--add-gps-to-you-meshtastic-node-(lora-device)-!)  as recognition just click on the star. 

Tutorial for use with meshtastic , device WIFI_LoRa_32_V2.1  (SX1276)

as V2 devices are using TP4054 wich seems by (generally) default has a 10k resistor on pin5 PROG
wich in turn sets charging current to onky 100mA if a liPo baterry is used to power the board

![TP4054_Iset](https://github.com/user-attachments/assets/a9fbdb11-3987-4524-9acf-0f513392b475)

Sollution is to change R9 to a smaller value 1.6k (or make a bridge with a wire, i do not advise tho unless no option left) wich will increase charging current to 600mAh
![alt text](https://github.com/yo8aiv/WIFI_LoRa_32_V2_charging_mod/blob/main/WIFI-LoRa-32-V2.1.png)

![alt text](https://github.com/yo8aiv/WIFI_LoRa_32_V2_charging_mod/blob/main/back.jpg)

 Also firmware wich seems to work with this version of hardware and settings right for baterry Voltage : V2.3.2 beta 
 
  (~~)Thanks to the dev's at -- > https://flasher.pdxlocs.com  (~~)

(~~)![alt test](https://github.com/yo8aiv/WIFI_LoRa_32_V2_charging_mod/blob/main/Meshtastic%20ESP32%20Web%20Installer.png)(~~)
 
>>  #define BATTERY_PIN 37 // A battery voltage measurement pin, voltage divider connected here to measure battery voltage
>> 
>>  #define ADC_CHANNEL ADC1_GPIO37_CHANNEL
>> 
>>  #define EXT_NOTIFY_OUT 13 // Default pin to use for Ext Notify Module.
>>
 you can build a custom bin if needed -- >  https://github.com/meshtastic/firmware/tree/master/variants/esp32/heltec_v2.1


keywords : heltec v2 gps connection, WIFI_LoRa_32_V2.1 gps connection, heltec v2.1 gps, heltec v2 firmware.








