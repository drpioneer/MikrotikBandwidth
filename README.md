# Bandwidth
Script of monitoring the channels between Mikrotik routers
Скрипт проверки ширины канала c использованием встроенного Bandwidth теста.
Для работы скрипта на дальнем конце канала должен быть настроен BandTestServer: Tools/BTestServer, Enabled=yes, Authenticate=yes.
В скрипте заполняется список каналов по шаблону:
name="имя_канала"; ip=ip_адрес_дальнего_конца;  user="имя_пользователя_для_bandwidth_теста";  pswd="пароль_для_bandwidth_теста"; prot="протокол_tcp_или_udp"
При запуске скрипта перебирается заданный список каналов и проводятся тесты. В конце выводится полученная статистика.
