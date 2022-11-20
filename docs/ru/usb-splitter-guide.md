# Руководство по сплиттеру USB/PWR

## **1. Введение**

![image-20220107110102815](assets/images/usb-splitter/usb-splitter.png)

Адаптер позволяет использовать Raspberry Pi 4 с блоком питания Pi USB-C, во время использования USB OTG через отдельное соединение USB-C.

USB-C (RPI4) <> USB-C (USB) и USB-C (PWR)

|   USB-C(RPI4)   |  USB Type-C(USB)  |  USB Type-C(PWR)  |
|:---------------:|:-----------------:|:-----------------:|
|       5V        |                   |        5V         |
|       D-        |        D-         |                   |
|       D+        |        D+         |                   |
|  CC1 10k в 5V   |  CC1 5.1k в GND   |   CC1 5.1k в GND  |
|  CC2 10k в 5V   |  CC2 5.1k в GND   |   CC2 5.1k в GND  |
|       GND       |        GND        |        GND        |

Для использования адаптера с Raspberry Pi 4 вам потребуется.

- Кабель USB-C в USB-C[1] между Pi4 и платой адаптера
- USB-C к USB-C или Type-A между платой адаптера и ПК
- Питание[2] через официальный источник питания Raspberry Pi USB Type-C

[1] Хотя кабели USB-C обычно рассчитаны на более высокий ток, рекомендуется использовать короткий кабель питания к Pi, где это возможно, чтобы уменьшить падение напряжения.

[2] **ОБРАТИТЕ ВНИМАНИЕ** С резисторами Pu/Pd на этой плате его можно использовать только с питанием 5 В для питания устройства 5 В.

Адаптер такого типа не подпадает под спецификацию USB. Он предназначается для использования с официальным источником питания Raspberry Pi USB-C и Raspberry Pi, использование с другими блоками питания/зарядными устройствами и другими устройствами может вызвать проблемы/повреждения.

## **2. Схема**

![image-20220107154909710](assets/images/usb-splitter/usb-splitter-size.png)

## **3. Видео с тестированием**

[USB сплиттер](https://www.youtube.com/watch?v=4Od5MjBHbhY)