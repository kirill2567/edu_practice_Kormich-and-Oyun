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
<img width="553" height="37" alt="image" src="https://github.com/user-attachments/assets/5de211f0-7062-41c6-a2df-09cb77b2c304" />
<img width="545" height="28" alt="image" src="https://github.com/user-attachments/assets/521ba20b-aed8-4ec5-8fd4-9776e27905fb" />

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


# Часть 2

## Шаг 1. Настройка интерфейса связи с Москвой 
<img width="596" height="146" alt="image" src="https://github.com/user-attachments/assets/0e706ae1-271e-47c4-9154-cebae16e0460" />

*Рис.21 Назначение IP-адреса на физ. интерфейс*

## Шаг 2. Настройка Router-on-a-Stick
<img width="629" height="477" alt="image" src="https://github.com/user-attachments/assets/5bf8d6d1-31e8-4231-b1e3-bf502f70ce05" />

*Рис.22 Настройка технологии Router-on-a-Stick на интерфейсе f0/0*

## Шаг 3. Настройка DHCP-сервера 
<img width="454" height="145" alt="image" src="https://github.com/user-attachments/assets/2d3e50e3-4689-4314-878e-b6321f347e25" />

*Рис.23 Настройка исключений IP-адресов для соблюдения диапозона*

<img width="325" height="246" alt="image" src="https://github.com/user-attachments/assets/6cc39f7b-0649-4aa3-8d02-48b025458194" />

*Рис.24 Настройка конфигурации DCHP-пулов*

## Шаг 4. Проверка связности (ping) 
<img width="427" height="235" alt="image" src="https://github.com/user-attachments/assets/0e37e4f5-5f2a-44c4-8a26-3c9c198e348f" />

*Рис.25 Проверка сетевого взаимодействия* 


# Часть 3

## Шаг 1. Настройка имени устройства 
<img width="440" height="74" alt="image" src="https://github.com/user-attachments/assets/f73a6ff0-4b29-4d2b-83be-fe9604a6a3dc" />

*Рис.26 Переименование устройства* 

## Шаг 2. Включение функций маршрутизации 
<img width="260" height="33" alt="image" src="https://github.com/user-attachments/assets/87d1e938-b8bf-499d-89a5-d11464f16eb8" />

*Рис.27 Активация функций маршрутизации 3-го уровня* 

## Шаг 3. Создание VLAN и назначение имён 
<img width="289" height="109" alt="image" src="https://github.com/user-attachments/assets/b32c733c-7a4b-42a2-85bc-ce059d37c7be" />

*Рис.28 Создание виртуальных локальных сетей* 

## Шаг 4. Назначение интерфейсов в VLAN 

<img width="366" height="127" alt="image" src="https://github.com/user-attachments/assets/b2191abb-a05d-4179-a682-f059319f37b0" />

*Рис.29 Настройка интерфейсов* 

## Шаг 5. Настройка межсетевой маршрутизации (SVI)*

<img width="581" height="268" alt="image" src="https://github.com/user-attachments/assets/f2f8029f-2006-46a1-b4a7-6855b53c4550" />

*Рис.30 Настройка виртальных интрейфесов коммутатора (SVI)*

## Шаг 6. Настройка интерфейсов 3-го уровня (Router Ports) 

<img width="605" height="270" alt="image" src="https://github.com/user-attachments/assets/43d5a945-c18f-4ea2-9d90-b3884c011e0f" />

*Рис.31 Перевод физ. портов 1,2,3 в режим интерфейсов 3-го уровня с помощью команды no switchport*

## Шаг 7. Проверка пингом устройств 

<img width="445" height="179" alt="image" src="https://github.com/user-attachments/assets/f6798430-0f92-4612-98c0-bf7494a9011c" />
<img width="324" height="123" alt="image" src="https://github.com/user-attachments/assets/797e3909-9f7c-44fe-a486-160a45f3daa5" />
<img width="428" height="206" alt="image" src="https://github.com/user-attachments/assets/fda0f801-c30a-460e-8bfd-81cda9892755" />

*Рис.32 Настройка IP на компьютере 6 и 7 и проверка пингом* 

# Часть 4

## Шаг 1. Конфигурация активного маршрутизатора R2

<img width="464" height="454" alt="image" src="https://github.com/user-attachments/assets/d6699d5e-5128-4609-bed1-e2d3d25536b0" />

*Рис.33 Настройка интерфейса fa0/1* 

## Шаг 2. Конфигурация резервного маршрутизатора R3

<img width="347" height="106" alt="image" src="https://github.com/user-attachments/assets/725cc722-4b83-40d6-b7a5-537ae6f83c6d" />

*Рис.34 Настройка R3 в качестве резервоного маршрутизатора* 

## Шаг 3. Настройка протокола Cisco High availability 

<img width="291" height="87" alt="image" src="https://github.com/user-attachments/assets/6edc2b67-984d-4803-9b33-e79589cd0a37" />
<img width="283" height="76" alt="image" src="https://github.com/user-attachments/assets/b11ebbeb-777c-4ce0-8e24-0fb60d642771" />

 *Рис.35, 36 Настройка Cisco High availability для r2 и r3*

# Часть 5

## Шаг 1. Настройка EIGRP 

На rus-nsk-r1

<img width="254" height="72" alt="image" src="https://github.com/user-attachments/assets/686ca5c2-f8c0-4fe1-840e-ab862be659cf" />

 *Рис.37 Настройка eigrp 100 на r1*

На rus-msk-r2 

<img width="255" height="100" alt="image" src="https://github.com/user-attachments/assets/3ec9937d-4e5c-48d9-98fb-c3f43557f609" />

 *Рис.38 Настройка eigrp 100 на r2*

На rus-msk-r3

<img width="643" height="129" alt="image" src="https://github.com/user-attachments/assets/2e856ae4-8b3a-489c-ab11-88bbc054adac" />

 *Рис.39 Настройка eigrp 100 на r3*

На rus-msk-mls

<img width="642" height="120" alt="image" src="https://github.com/user-attachments/assets/05041505-d6c6-4f2f-8d4d-639fb3d23ffd" />

 *Рис.40 Настройка eigrp 100 на mls*

## Шаг 2. Проверка с помощью SSH

<img width="305" height="104" alt="image" src="https://github.com/user-attachments/assets/99708d51-e87b-4504-b275-f252799fd9e1" />
<img width="320" height="110" alt="image" src="https://github.com/user-attachments/assets/d6b67e42-4bce-4360-90fe-36dccb0b00f3" />

 *Рис.41, 42 Подключение sw1 и sw2 на сервере*

## Шаг 3. Пропинговать с сервера 

<img width="403" height="193" alt="image" src="https://github.com/user-attachments/assets/3b4dddcf-aa36-47e9-bd71-6970985a23cf" />

 *Рис.43 Проверка подключения*

# Часть 6

## Шаг 1. Настройка SW 1,2  

<img width="434" height="180" alt="image" src="https://github.com/user-attachments/assets/01370bec-4644-4baf-8739-41492d9047d0" />
<img width="350" height="140" alt="image" src="https://github.com/user-attachments/assets/c4cf73be-8843-46d8-85a5-d09c23004056" />

 *Рис.44 Ограничение ssh на sw 1,2*

## Шаг 2. Настройка доступа к WEB-серверу

<img width="475" height="241" alt="image" src="https://github.com/user-attachments/assets/205dd300-cef7-44d2-a99c-dbfef03013db" />

 *Рис.45 Доступ к web-серверу на r1* 

## Шаг 3. Запрет ответа на PING 

<img width="376" height="193" alt="image" src="https://github.com/user-attachments/assets/c418cd99-7cb2-4445-8c2f-69f432efc275" />
<img width="376" height="187" alt="image" src="https://github.com/user-attachments/assets/35eb6b69-487a-4bd7-87cd-36a34e56c231" />

  *Рис.46 Запрет на пинг* 
  
# Часть 7

## Шаг 1. Создание Loopbakc-интерфейса 

<img width="554" height="184" alt="image" src="https://github.com/user-attachments/assets/2c6daccd-9798-4b95-8492-6193946ba7b6" />

 *Рис.47 Loopback на r1*

## Шаг 2. Создание Loopbakc-интерфейса 

<img width="559" height="200" alt="image" src="https://github.com/user-attachments/assets/32489f50-df2d-40f1-9ae2-4d45d0c9cf28" />

 *Рис.48 Loopback на r3* 

## Шаг 3. Настройка RIPv2 

<img width="277" height="99" alt="image" src="https://github.com/user-attachments/assets/2cb4e9c6-4d3e-4773-abe4-9870f1d4d041" />
<img width="291" height="99" alt="image" src="https://github.com/user-attachments/assets/cfffb68f-d090-4043-bab7-a9649f99ef01" />

 *Рис.49 Настройка RIPv2 на r1 и r3* 

## Шаг 4.

<img width="183" height="13" alt="image" src="https://github.com/user-attachments/assets/d674d280-1cb5-44c2-9652-8a8c172717c9" />
<img width="245" height="21" alt="image" src="https://github.com/user-attachments/assets/c2426b17-3569-4a44-ac2f-64034b76d4e9" />


## Шаг 5. IP адреса для туннелей 

<img width="536" height="158" alt="image" src="https://github.com/user-attachments/assets/bdd2e351-f6ca-4211-a96e-f2278e5f005f" />
<img width="556" height="191" alt="image" src="https://github.com/user-attachments/assets/d2c267ad-9de2-4e87-89ab-2cd0eaf8ac17" />

 *Рис.50 настройка IP-адреса для туннелей на r1 и r3* 

## Шаг 6.



<img width="607" height="331" alt="image" src="https://github.com/user-attachments/assets/a853c5a3-1771-4167-aa22-a951e2781548" />


<img width="536" height="339" alt="image" src="https://github.com/user-attachments/assets/5ebb3e82-26c9-452a-9a04-487276adbd4d" />


<img width="525" height="337" alt="image" src="https://github.com/user-attachments/assets/dd29b689-975d-4ba7-bf50-ba360874c285" />


<img width="524" height="329" alt="image" src="https://github.com/user-attachments/assets/8c2ac749-e43f-42c0-aee0-b79dcc010e68" />


<img width="588" height="334" alt="image" src="https://github.com/user-attachments/assets/ade5021a-ec08-4dc7-8455-6d5aa5224333" />


<img width="561" height="336" alt="image" src="https://github.com/user-attachments/assets/61144ccc-e006-498c-8008-5cc31e227ff7" />


<img width="529" height="347" alt="image" src="https://github.com/user-attachments/assets/e6d2ff85-f6d9-4d26-bb0d-319846b6c482" />


<img width="470" height="333" alt="image" src="https://github.com/user-attachments/assets/b10158ca-3506-4c1a-b62f-67e688c3bc2d" />


rus-msk-r3
```
!
version 15.1
no service timestamps log datetime msec
no service timestamps debug datetime msec
no service password-encryption
!
hostname R2
!
!
!
enable secret 5 $1$mERr$hx5rVt7rPNoS4wqbXKX7m0
!
!
!
!
!
aaa new-model
!
aaa authentication login TELNET_AUTH group radius local 
!
!
!
!
!
!
!
no ip cef
no ipv6 cef
!
!
!
username newadmin secret 5 $1$mERr$y1xCpu9vTanV1oFENCDrX0
username standby secret 5 $1$mERr$hx5rVt7rPNoS4wqbXKX7m0
!
!
license udi pid CISCO2811/K9 sn FTX10177M0D-
!
!
!
!
!
!
!
!
!
ip domain-name msk.local
!
!
spanning-tree mode pvst
!
!
!
!
!
!
interface Loopback0
 ip address 192.168.103.3 255.255.255.0
!
interface Tunnel0
 ip address 200.200.200.3 255.255.255.0
 mtu 1476
 tunnel source FastEthernet0/0
 tunnel destination 40.40.40.1
!
!
interface FastEthernet0/0
 ip address 10.0.0.3 255.0.0.0
 ip access-group 120 in
 duplex auto
 speed auto
 standby 1 ip 10.0.0.1
 standby 1 preempt
!
interface FastEthernet0/1
 ip address 12.0.0.3 255.0.0.0
 ip access-group 120 in
 duplex auto
 speed auto
!
interface Vlan1
 no ip address
 shutdown
!
router eigrp 100
 network 10.0.0.0
 network 12.0.0.0
!
router rip
 version 2
 network 192.168.103.0
 network 200.200.200.0
 no auto-summary
!
ip classless
!
ip flow-export version 9
!
!
access-list 120 permit icmp any any echo-reply
access-list 120 deny icmp any any echo
access-list 120 permit ip any any
!
banner motd Work is create Kormich Kirill Evgenevich and Oyun Ertine Viktorovich students is 9SA-321 group in the magazine under the number 14 and 19




banner motd W
!
radius server 10.0.0.100
 address ipv4 10.0.0.100 auth-port 1645
 key cisco
!
!
snmp-server community cisco RW
!
logging 10.0.0.100
line con 0
!
line aux 0
!
line vty 0 4
 login authentication TELNET_AUTH
 transport input telnet
!
!
ntp authentication-key 1 md5 0822455D0A16 7
ntp authenticate
ntp trusted-key 1
ntp server 10.0.0.100 key 1
!
end
```

rus-msk-r2
```
!
version 12.2(37)SE1
no service timestamps log datetime msec
no service timestamps debug datetime msec
no service password-encryption
!
hostname rus-msk-mls
!
!
!
!
!
!
ip routing
!
!
!
!
!
!
!
!
!
!
!
!
!
!
!
spanning-tree mode pvst
!
!
!
!
!
!
interface FastEthernet0/1
 no switchport
 ip address 11.0.0.50 255.0.0.0
 duplex auto
 speed auto
!
interface FastEthernet0/2
 no switchport
 ip address 12.0.0.50 255.0.0.0
 duplex auto
 speed auto
!
interface FastEthernet0/3
 no switchport
 ip address 40.40.40.50 255.255.255.0
 duplex auto
 speed auto
!
interface FastEthernet0/4
 switchport access vlan 100
 switchport mode access
!
interface FastEthernet0/5
 switchport access vlan 200
 switchport mode access
!
interface FastEthernet0/6
!
interface FastEthernet0/7
!
interface FastEthernet0/8
!
interface FastEthernet0/9
!
interface FastEthernet0/10
!
interface FastEthernet0/11
!
interface FastEthernet0/12
!
interface FastEthernet0/13
!
interface FastEthernet0/14
!
interface FastEthernet0/15
!
interface FastEthernet0/16
!
interface FastEthernet0/17
!
interface FastEthernet0/18
!
interface FastEthernet0/19
!
interface FastEthernet0/20
!
interface FastEthernet0/21
!
interface FastEthernet0/22
!
interface FastEthernet0/23
!
interface FastEthernet0/24
!
interface GigabitEthernet0/1
!
interface GigabitEthernet0/2
!
interface Vlan1
 no ip address
 shutdown
!
interface Vlan100
 mac-address 000c.cf1e.8501
 ip address 100.0.0.50 255.0.0.0
!
interface Vlan200
 mac-address 000c.cf1e.8502
 ip address 200.0.0.50 255.255.255.0
!
router eigrp 100
 network 11.0.0.0
 network 12.0.0.0
 network 40.40.40.0 0.0.0.255
 network 100.0.0.0
 network 200.0.0.0
 no auto-summary
!
ip classless
!
ip flow-export version 9
!
!
!
!
!
!
!
!
line con 0
!
line aux 0
!
line vty 0 4
 login
!
!
!
!
end
```

rus-msk-mls
```
!
version 12.2(37)SE1
no service timestamps log datetime msec
no service timestamps debug datetime msec
no service password-encryption
!
hostname rus-msk-mls
!
!
!
!
!
!
ip routing
!
!
!
!
!
!
!
!
!
!
!
!
!
!
!
spanning-tree mode pvst
!
!
!
!
!
!
interface FastEthernet0/1
 no switchport
 ip address 11.0.0.50 255.0.0.0
 duplex auto
 speed auto
!
interface FastEthernet0/2
 no switchport
 ip address 12.0.0.50 255.0.0.0
 duplex auto
 speed auto
!
interface FastEthernet0/3
 no switchport
 ip address 40.40.40.50 255.255.255.0
 duplex auto
 speed auto
!
interface FastEthernet0/4
 switchport access vlan 100
 switchport mode access
!
interface FastEthernet0/5
 switchport access vlan 200
 switchport mode access
!
interface FastEthernet0/6
!
interface FastEthernet0/7
!
interface FastEthernet0/8
!
interface FastEthernet0/9
!
interface FastEthernet0/10
!
interface FastEthernet0/11
!
interface FastEthernet0/12
!
interface FastEthernet0/13
!
interface FastEthernet0/14
!
interface FastEthernet0/15
!
interface FastEthernet0/16
!
interface FastEthernet0/17
!
interface FastEthernet0/18
!
interface FastEthernet0/19
!
interface FastEthernet0/20
!
interface FastEthernet0/21
!
interface FastEthernet0/22
!
interface FastEthernet0/23
!
interface FastEthernet0/24
!
interface GigabitEthernet0/1
!
interface GigabitEthernet0/2
!
interface Vlan1
 no ip address
 shutdown
!
interface Vlan100
 mac-address 000c.cf1e.8501
 ip address 100.0.0.50 255.0.0.0
!
interface Vlan200
 mac-address 000c.cf1e.8502
 ip address 200.0.0.50 255.255.255.0
!
router eigrp 100
 network 11.0.0.0
 network 12.0.0.0
 network 40.40.40.0 0.0.0.255
 network 100.0.0.0
 network 200.0.0.0
 no auto-summary
!
ip classless
!
ip flow-export version 9
!
!
!
!
!
!
!
!
line con 0
!
line aux 0
!
line vty 0 4
 login
!
!
!
!
end
```

rus-nsk-sw2
```
!
version 15.0
no service timestamps log datetime msec
no service timestamps debug datetime msec
no service password-encryption
!
hostname SW1
!
!
!
ip domain-name msk.local
!
!
!
spanning-tree mode pvst
spanning-tree extend system-id
!
interface FastEthernet0/1
!
interface FastEthernet0/2
!
interface FastEthernet0/3
!
interface FastEthernet0/4
!
interface FastEthernet0/5
!
interface FastEthernet0/6
!
interface FastEthernet0/7
!
interface FastEthernet0/8
!
interface FastEthernet0/9
!
interface FastEthernet0/10
!
interface FastEthernet0/11
!
interface FastEthernet0/12
!
interface FastEthernet0/13
!
interface FastEthernet0/14
!
interface FastEthernet0/15
!
interface FastEthernet0/16
!
interface FastEthernet0/17
!
interface FastEthernet0/18
!
interface FastEthernet0/19
!
interface FastEthernet0/20
!
interface FastEthernet0/21
!
interface FastEthernet0/22
!
interface FastEthernet0/23
!
interface FastEthernet0/24
!
interface GigabitEthernet0/1
!
interface GigabitEthernet0/2
!
interface Vlan1
 no ip address
 shutdown
!
!
!
!
line con 0
!
line vty 0 4
 login
line vty 5 15
 login
!
!
!
!
end
```


rus-nsk-sw1
```
!
version 15.0
no service timestamps log datetime msec
no service timestamps debug datetime msec
no service password-encryption
!
hostname SW1
!
!
!
ip ssh version 2
ip domain-name nsk.local
!
username nsk secret 5 $1$mERr$hx5rVt7rPNoS4wqbXKX7m0
!
!
!
spanning-tree mode pvst
spanning-tree extend system-id
!
interface Port-channel1
 switchport mode trunk
!
interface FastEthernet0/1
 shutdown
!
interface FastEthernet0/2
 switchport access vlan 2
 switchport mode access
 switchport port-security mac-address sticky 
 no cdp enable
 spanning-tree portfast
 spanning-tree bpduguard enable
!
interface FastEthernet0/3
 switchport access vlan 3
 switchport mode access
 switchport port-security mac-address sticky 
 no cdp enable
 spanning-tree portfast
 spanning-tree bpduguard enable
!
interface FastEthernet0/4
 switchport access vlan 4
 switchport mode access
 switchport port-security mac-address sticky 
 no cdp enable
 spanning-tree portfast
 spanning-tree bpduguard enable
!
interface FastEthernet0/5
!
interface FastEthernet0/6
!
interface FastEthernet0/7
!
interface FastEthernet0/8
!
interface FastEthernet0/9
!
interface FastEthernet0/10
!
interface FastEthernet0/11
!
interface FastEthernet0/12
!
interface FastEthernet0/13
!
interface FastEthernet0/14
!
interface FastEthernet0/15
!
interface FastEthernet0/16
!
interface FastEthernet0/17
!
interface FastEthernet0/18
!
interface FastEthernet0/19
!
interface FastEthernet0/20
!
interface FastEthernet0/21
!
interface FastEthernet0/22
!
interface FastEthernet0/23
!
interface FastEthernet0/24
!
interface GigabitEthernet0/1
 switchport mode trunk
 channel-group 1 mode passive
!
interface GigabitEthernet0/2
 switchport mode trunk
 channel-group 1 mode passive
!
interface Vlan1
 no ip address
 shutdown
!
interface Vlan2
 ip address 2.0.0.50 255.0.0.0
!
ip default-gateway 2.0.0.1
!
banner motd #This is a switchboard named rus-nsk-sw1#
!
!
!
access-list 10 permit host 10.0.0.100
access-list 10 permit host 2.0.0.100
line con 0
 logging synchronous
 login local
 history size 256
 exec-timeout 0 0
!
line vty 0 4
 access-class 10 in
 exec-timeout 0 0
 login local
 transport input ssh
line vty 5 15
 access-class 10 in
 exec-timeout 0 0
 login local
 transport input ssh
!
!
!
!
end
```

rus-nsk-sw0
```
!
version 15.0
no service timestamps log datetime msec
no service timestamps debug datetime msec
no service password-encryption
!
hostname SW0
!
!
!
ip ssh version 2
ip domain-name nsk.local
!
username nsk secret 5 $1$mERr$hx5rVt7rPNoS4wqbXKX7m0
!
!
!
spanning-tree mode pvst
spanning-tree extend system-id
!
interface Port-channel1
 switchport mode trunk
!
interface FastEthernet0/1
!
interface FastEthernet0/2
 switchport access vlan 2
 switchport mode access
 switchport port-security mac-address sticky 
 no cdp enable
 spanning-tree portfast
 spanning-tree bpduguard enable
!
interface FastEthernet0/3
 switchport access vlan 3
 switchport mode access
 switchport port-security mac-address sticky 
 no cdp enable
 spanning-tree portfast
 spanning-tree bpduguard enable
!
interface FastEthernet0/4
 switchport access vlan 4
 switchport mode access
 switchport port-security mac-address sticky 
 no cdp enable
 spanning-tree portfast
 spanning-tree bpduguard enable
!
interface FastEthernet0/5
!
interface FastEthernet0/6
!
interface FastEthernet0/7
!
interface FastEthernet0/8
!
interface FastEthernet0/9
!
interface FastEthernet0/10
!
interface FastEthernet0/11
!
interface FastEthernet0/12
!
interface FastEthernet0/13
!
interface FastEthernet0/14
!
interface FastEthernet0/15
!
interface FastEthernet0/16
!
interface FastEthernet0/17
!
interface FastEthernet0/18
!
interface FastEthernet0/19
!
interface FastEthernet0/20
!
interface FastEthernet0/21
!
interface FastEthernet0/22
!
interface FastEthernet0/23
!
interface FastEthernet0/24
 switchport mode trunk
!
interface GigabitEthernet0/1
 switchport mode trunk
 channel-group 1 mode active
!
interface GigabitEthernet0/2
 switchport mode trunk
 channel-group 1 mode active
!
interface Vlan1
 ip address 1.0.0.50 255.0.0.0
!
ip default-gateway 1.0.0.1
!
banner motd #This is a switchboard named rus-nsk-sw0#
!
!
!
access-list 10 permit host 10.0.0.100
access-list 10 permit host 2.0.0.100
line con 0
 logging synchronous
 login local
 history size 256
 exec-timeout 0 0
!
line vty 0 4
 access-class 10 in
 exec-timeout 0 0
 login local
 transport input ssh
line vty 5 15
 access-class 10 in
 exec-timeout 0 0
 login local
 transport input ssh
!
!
!
!
end
```
  


