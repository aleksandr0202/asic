Пользовательская прошивка для всех Antminer серии S19 без DevFee
=============

✅СКАЧАТЬ АРХИВ ПРОШИВКИ https://disk.yandex.ru/d/ywkAz9AafkYzqg

🤖Инструкции по установке https://vnish.pro/ru/documentation/64-install-vnish-firmware.html
------------------

Чтобы собрать прошивку для майнера bitmainer, сначала подготовьте сборочный компьютер в соответствии с инструкциями по установке необходимого программного обеспечения OpenEmbedded на http://www.openembedded.org/wiki/Getting_started

После подготовки компьютера приступайте к сборке прошивки bitmainer.

    git clone git@github.com:bitmaintech/Antminer_firmware.git
    cd antminer_firmware
    MACHINE=beaglebone ./oebb.sh config beaglebone

Инструкции по сборке Rootfs
----------------------------------

Чтобы собрать корневую файловую систему прошивки, выполните команду

    . environment-angstrom-v2013.06
    bitbake virtual/kernel

В результате получается изображение ядра

Примечание: вам потребуется около 11 ГБ свободного места на диске.

Результирующий корневой файл initramfs будет находиться в

    antminer_firmware/deploy/eglibc/images/beaglebone/Angstrom-bitmainer-eglibc-ipk-v2013.06-beaglebone.rootfs.cpio.gz.u-boot


Инструкции по сборке ядра
-----------------------------------

Чтобы создать образ ядра Linux, запустите

    . environment-angstrom-v2013.06
    bitbake virtual/kernel

что приводит к созданию образа ядра по адресу

    antminer_firmware/deploy/eglibc/images/beaglebone/

-----------------------------------
📜Отказ от ответственности
-----------------------------------
✅Автор не несет ответственности за неправомерное использование этого скрипта. Помните, что атака на цели без предварительного согласования является незаконной и преследуется по закону. Этот скрипт был создан, чтобы показать, как автоматизировать процесс брутфорса.
-----------------------------------
