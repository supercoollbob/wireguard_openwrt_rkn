# wireguard_openwrt_rkn
Простой скрипт для openwrt, на базе wireguard, для обхода блокировок роскомнадзор(ркн).

Настройка сервера.
Необходим VPS или аналог, рекомендую https://www.hetzner.com/cloud, не Xen, полная виртуализация, да и Финляндия близко к Россси, и траффик почти безлимитный в отличие от кункурентов.
Зайти по ssh  и выполнить "wget https://git.io/wireguard -O wireguard-install.sh && bash wireguard-install.sh"
В паке /root оразуются конфиги клиентов

Либо можно использовать любой иной сервис.
Проблема в том, что поддержка wireguard пристуствует только в последних linux ядрах, готового пакета для linux дистрибутивов нет.
Но есть простое решение https://d.sb/2019/07/wireguard-on-openvz-lxc , память фиксить обязательно(device/queueconstants_default)!!!
Это рализация wireguard на языке go, от производителя.


