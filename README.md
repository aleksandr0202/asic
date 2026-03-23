Пользовательская прошивка для всех Antminer серии S19 без DevFee
=============

✅СКАЧАТЬ АРХИВ ПРОШИВКИ https://disk.yandex.ru/d/ywkAz9AafkYzqg

🤖Инструкции по установке https://vnish.pro/ru/documentation/64-install-vnish-firmware.html
------------------

TЧтобы собрать прошивку для майнера bitmainer, сначала подготовьте сборочный компьютер в соответствии с инструкциями по установке необходимого программного обеспечения OpenEmbedded на http://www.openembedded.org/wiki/Getting_started

После подготовки компьютера приступайте к сборке прошивки bitmainer.
    git clone git@github.com:bitmaintech/Antminer_firmware.git
    cd antminer_firmware
    MACHINE=beaglebone ./oebb.sh config beaglebone

Инструкции по сборке Rootfs
----------------------------------

Чтобы собрать корневую файловую систему прошивки, выполните команду

    . environment-angstrom-v2013.06
    bitbake bitmainer

and then wait for quite a bit for the build to complete.

Note: You will need ~11GB free disk space.

The resulting root initramfs will be in

    antminer_firmware/deploy/eglibc/images/beaglebone/Angstrom-bitmainer-eglibc-ipk-v2013.06-beaglebone.rootfs.cpio.gz.u-boot


Kernel build instructions
-----------------------------------

To build the Linux kernel image run

    . environment-angstrom-v2013.06
    bitbake virtual/kernel

which results in a kernel image at

    antminer_firmware/deploy/eglibc/images/beaglebone/

-----------------------------------
📜License с ограничениями
-----------------------------------
РАЗРЕШЕНО:
✅ Личное использование в образовательных целях
✅ Модификация исходного кода
✅ Форки репозитория
-----------------------------------
ЗАПРЕЩЕНО:
❌ Коммерческое использование
❌ Распространение в странах с запретом VPN
❌ Использование для незаконной деятельности
-----------------------------------
АВТОР НЕ НЕСЁТ ОТВЕТСТВЕННОСТИ ЗА:
⚠️ Действия пользователей
⚠️ Нарушение законодательства
⚠️ Утечки данных
-----------------------------------
