# RFFE-SVCh-KIT
Пример сборки РЧИ для ПКР на основе блоков СВЧ КИТ



## Порядок прошивки:
1) Распакуйте архив MCC01B.zip
<p align="center">
  <img width="" height="" src="/media/firmware.png">
</p>
2) Запустите приложение Keil uVision5 и откройте проект, выбрав файл Blank.uvprojx <br>
3) Зайдите в настройки проекта, открыв "Options for target" в меню "Project"<br>
 <p align="center">
  <img width="" height="" src="/media/firmware2.png">
</p>
4) Перейдите во вкладку "Utilities". Выберите "Use Target Driver for Flash Programming, а затем выберите из списка ваш программатор (Для данного примера это ST-Link). Поставьте галочку напротив "Update Target before Debugging"
 <p align="center">
  <img width="" height="" src="/media/firmware4.png">
</p>
5) В меню Debug выберите опцию "Use:", выберите необходимый debugger, в качестве примера это ST-Link Debugger
 <p align="center">
  <img width="" height="" src="/media/firmware6.png">
</p>
6) В меню Device выберите необходимый микроконтроллер по пути Milandr/Milandr/Cortex-M3/MDR32F9Q2I. Нажмите OK
 <p align="center">
  <img width="" height="" src="/media/firmware5.png">
</p>
7) Подсоедините программатор к плате DC-MCC01B-16 через четыре порта для пого-пинов, подключите питание через разъем USB Type C
<p align="center">
  <img width="" height="" src="/media/firmware2.jpg">
</p>
8) В верхней строке выберите сначала "Build", затем "Download"
 <p align="center">
  <img width="" height="" src="/media/firmware3.png">
</p>
9) После этого плата будет прошита

---

## Порядок установки:
1) Распакуйте архив app.zip
<p align="center">
  <img width="" height="" src="/media/app install.png">
</p>
2) Запустите setup.exe<br>
3) В окне с предупреждением выберите "Install"
<p align="center">
  <img width="" height="" src="/media/app install2.png">
</p>
4) Сразу после установки откроется приложение
<p align="center">
  <img width="" height="" src="/media/app install3.png">
</p>

---

## Подключение к микроконтроллеру
1) Подключите плату микроконтроллера к компьютеру <br>
2) Нажмите кнопку "Обновить", после чего откройте выпадающий список и выберите необходимый COM-порт (Убедиться в том, что выбранный COM-порт относится к микроконтроллеру, можно в диспетчере устройств Windows)
<p align="center">
  <img width="" height="" src="/media/app install4.png">
</p>
3) Нажмите "Подключиться". Если все сделано верно, появится надпись "Подключен к порту COMX", и строка загорится зеленым цветом. Если этого не произошло, попробуйте переподключить микроконтроллер и повторить снова.
<p align="center">
  <img width="" height="" src="/media/app install5.png">
</p>
4) В случае, если в процессе работы строка изменит цвет на красный с надписью "Соединение разорвано", нажмите "Отключиться", затем переподключите микроконтроллер и повторите шаг 2
<p align="center">
  <img width="" height="" src="/media/app install6.png">
</p>
