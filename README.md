#  Базовая настройка коммутатора

------------



###  Задание:
###### **Часть 1. Проверка конфигурации коммутатора по умолчанию** 
###### **Часть 2. Создание сети и настройка основных параметров устройства**



- Разработать и задокументировать адресное пространство
- Настроить IP адреса на каждом активном порту

###### **Часть 3. Проверка сетевых подключений**

  - Отобразите конфигурацию устройства
  - Протестируйте сквозное соединение, отправив эхо-запрос.
  - Протестируйте возможности удаленного управления с помощью Telnet.
  
###  	Общие сведения/сценарий



 На коммутаторах Cisco можно настроить особый IP-адрес, который называют виртуальным интерфейсом коммутатора (SVI). SVI или адрес управления можно использовать для удаленного доступа к коммутатору в целях отображения или настройки параметров. Если для SVI сети VLAN 1 назначен IP-адрес, то по умолчанию все порты в сети VLAN 1 имеют доступ к IP-адресу управления SVI.
 В ходе данной лабораторной работы вам предстоит построить простую топологию, используя Ethernet-кабель локальной сети, и получить доступ к коммутатору Cisco, используя консольное подключение и методы удаленного доступа. Перед настройкой базовых параметров коммутатора нужно проверить настройки коммутатора по умолчанию. В число таких основных параметров коммутации входят имя устройства, описание интерфейса, локальные пароли, объявление дня (MOTD), IP-адрес и статический MAC-адрес. Необходимо также показать использование IP-адреса управления для удаленного управления коммутатором. Топология включает один коммутатор и один узел с использованием только портов Ethernet и консольных портов.
 __Примечание__. В лабораторной работе используются коммутаторы Cisco Catalyst 2960s с операционной системой Cisco IOS 15.2(2) (образ lanbasek9). Допускается использование других моделей коммутаторов и других версий Cisco IOS. В зависимости от модели устройства и версии Cisco IOS доступные команды и результаты их выполнения могут отличаться от тех, которые показаны в лабораторных работах.
 __Примечание__. Убедитесь, что все настройки коммутатора удалены и загрузочная конфигурация отсутствует. Если вы не уверены, обратитесь к инструктору. Процедура инициализации и перезагрузки коммутатора описана в приложении А
 
 ###Часть 1. Создание сети и проверка настроек коммутатора по умолчанию
   В первой части работы нам нужно настроить топологию сети и проверить настройку коммутатора по умолчанию.
   
   #### Топологическая схема. Рисунок 1.
  
   
   
   
   #### Шаг1.Создаем сеть согласно топологии.
- Подсоединяем консольный кабелькак показано в топологии (рисунок1). На данном этапе не подключаем кабель Ethernet компьютера PC-A.
- Устанавливаем консольное подключение к коммутатору с компьютера PC-A с помощью Tera Term или другой программы эмуляции терминала

