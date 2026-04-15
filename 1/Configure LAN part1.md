# Часть 1
## Шаг 1. Построили сеть с топологией согласно схеме. 
<img width="2122" height="868" alt="image" src="https://github.com/user-attachments/assets/c40b8c73-b46e-4583-b791-298a5bbbfc3f" />
*Рис.1 Топология сети*

## Шаг 2. Создали сообщение дня banner motd "Work is create Kormich Kirill Evgenevich and Oyun Ertine Viktorovich students is 9SA-321 group in the magazine under the number 14 and 19"
<img width="793" height="272" alt="image" src="https://github.com/user-attachments/assets/918801ef-5b20-43df-afca-b82e5888e48b" />
*Рис.2 Настройка баннера на маршрутизаторах*

## Шаг 3. Переименуем все устройства (например rus-nsk-pc1)
<img width="576" height="182" alt="image" src="https://github.com/user-attachments/assets/0e3e5f1e-adc1-4ce1-809b-6319afcde705" />
*Рис.3 Изменение имени хоста согласно шаблону*

## Шаг 4. Раздаём доменные имена устройствам 
<img width="410" height="75" alt="image" src="https://github.com/user-attachments/assets/1d1c62a9-47a6-4089-9b5a-116d78ea3cd8" />
<img width="464" height="58" alt="image" src="https://github.com/user-attachments/assets/71b906ed-0485-43bd-9166-b4485689f701" />
*Рис.4,5 Назначение доменного имени устройствам*

## Шаг 5-6. На коммутаторах в Новосибирске создаем vlan 2,3,4 без присваниваний имён
<img width="420" height="253" alt="image" src="https://github.com/user-attachments/assets/17d61165-037a-4c7a-ab0c-a0524be6f026" />
*Рис.6 Создание виртуальных локальных сетей*

## Шаг 7. Создание канала EtherChannel 2-го уровня 
<img width="820" height="419" alt="image" src="https://github.com/user-attachments/assets/8a2905eb-252f-4720-a445-77d5b69f7b24" />
<img width="750" height="453" alt="image" src="https://github.com/user-attachments/assets/d1d35c6a-4dd6-48bb-9947-22001eb239ab" />
*Рис.7,8 Агрегирование физических каналов в логический интерфейс*

## Шаг 8. Создаем Management interface на SW0
<img width="597" height="203" alt="image" src="https://github.com/user-attachments/assets/2283d8b6-ccff-44d7-80aa-a2aaf89c3556" />
*Рис.9 Настройка IP-адреса на интерфейсе управления и указание шлюза* 

## Шаг 9. Создаем Management interface на SW1
<img width="610" height="246" alt="image" src="https://github.com/user-attachments/assets/aa65c428-b17d-4dd0-8670-b5c846dba6ea" />
*Рис.10 Настройка IP-адреса на интерфейсе управления и указание шлюза*

## Шаг 10. Включаем SSHv2 на коммутаторах в Новосибирске 
<img width="613" height="274" alt="image" src="https://github.com/user-attachments/assets/f29f8c35-169c-4d55-a996-d98814289507" />
<img width="589" height="271" alt="image" src="https://github.com/user-attachments/assets/d23a6bb9-d9d4-4688-a65f-c48b75f6e2a9" />
*Рис.11,12 Активация протокла SHH версии 2*

## Шаг 11. Настройка транка к роутеру (SW0)
<img width="315" height="114" alt="image" src="https://github.com/user-attachments/assets/9db04132-48e8-4772-bcc6-3de49585c303" />
*Рис.13 Перевод интерфейса в режим транка*

## Шаг 12. Настройка динамического MOTD для SW0 и SW1 
<img width="566" height="36" alt="image" src="https://github.com/user-attachments/assets/1f3a151c-1d02-480b-840d-8e1030834d46" />
<img width="519" height="39" alt="image" src="https://github.com/user-attachments/assets/6d096c0e-c0ef-4f49-b149-3acce0194d98" />
*Рис.14,15 Настройка динамического баннера*

## Шаг 13. Настройка безопасности портов (PortSecurity) на SW0 и SW1
<img width="597" height="490" alt="image" src="https://github.com/user-attachments/assets/9b229db1-8ee7-460f-aa65-c37ed2891f57" />  <img width="565" height="578" alt="image" src="https://github.com/user-attachments/assets/a350cff6-acc1-429d-8675-4e5bb53710df" />
*Рис.16 Настройка ускоренного перехода в режим пересылки, защита от петель, ограничение по MAC-адресам

## Шаг 14. Защита консольного подключения(на всех устройствах)
<img width="285" height="70" alt="image" src="https://github.com/user-attachments/assets/638f9fa0-850d-47eb-9fee-e2445ac9a8f2" />
*Рис.17 Настройка ауентификации для консольного порта*

## Шаг 15. Откючение тайм-аута сессии(на всех устройствах)
<img width="315" height="98" alt="image" src="https://github.com/user-attachments/assets/6534de0c-8ad1-4622-80dd-f148a4b2702f" />
*Рис.18 Отключение автоматического завершения сессии при бездейтсвии*

## Шаг 16. Предотвращение прерывания ввода(на всех устройствах) 
<img width="314" height="124" alt="image" src="https://github.com/user-attachments/assets/5aa65486-926a-4107-8c75-af72b8f70674" />
*Рис.19 Настройка синхронного вывода системных сообщений*

## Шаг 17. Размер буфера истории(на всех устройствах) 
<img width="309" height="137" alt="image" src="https://github.com/user-attachments/assets/19287367-10d8-431e-827d-2ed1e83d9ad8" />
*Рис.20 Увеличение размера буфера истории команд до 256и строк*





