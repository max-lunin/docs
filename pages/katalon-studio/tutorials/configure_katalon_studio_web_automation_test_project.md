---
title: "Конфигурирование Katalon Studio для Веб-тестирования"
sidebar: katalon_studio_tutorials_sidebar
permalink: katalon-studio/tutorials/configure_katalon_studio_web_automation_test_project.html
description: "Katalon Studio поддерживает функциональное тестирование веб-приложений во многих браузерах. Этот урок объясняет как настроить тестовый проект в Katalon Studio."
---
Katalon Studio поддерживает функциональное тестирование веб-приложений в Internet Explorer, Edge, Chrome, Firefox and Safari.

Этот урок объясняет как настроить тестовый проект в Katalon Studio. Мы предполагаем, что вы знакомы с общими принципами автоматизированного тестирования и имеете минимальные знания Katalon Studio.

Конфигурация Internet Explorer
------------------------------

Пропустите этот раздел если вы не хотите запускать ваши автоматизированные тесты в Internet Expolorer. В противном случае, вам необходимо сделать следующие настройки:

– Для версий IE 7 - IE 11, установите одинаковое значение уровня **Безопасности** для всех зон (_Интернет, Местная интрасеть, Надежные сайты_ и _Опасные сайты_). Чтобы получить доступ к настройкам, выберите **Свойства браузера** в **Панели управления** Windows, затем переключитесь на вкладку **Безопасность**:

![Internet Options](../../images/katalon-studio/tutorials/configure_katalon_studio_web_automation_test_project/1.-Katalon-Security.png)

– Для IE 10 и более поздних версий, снимите галочку с чекбокса **Включить расширенный защищенный режим*** на вкладке **Дополнительно**.

![Enable Enhanced Protected Mode](../../images/katalon-studio/tutorials/configure_katalon_studio_web_automation_test_project/2.-Katalon-Security.png)

– Установите значение **Масштаб** IE в **100%**, чтобы события мыши могли быть корректно идентифицированы.

![Zoom level on IE for web automation](../../images/katalon-studio/tutorials/configure_katalon_studio_web_automation_test_project/3.-Katalon-IE.png)

– Для IE 11, вам необходимо сделать запись в реестре на целевом компьютере чтобы драйвер Katalon мог поддерживать соединение с экземплярами IE, которые он создает.

1. Наберите '**_regedit_**' в **командной строке**, чтобы открыть **Редактор реестра**.

2\. Найдите подключ **FEATURE_BFCACHE** (создайте подключ **FEATURE_BFCACHE** если он не существует):

2.1 Для 32-битной Windows этот подключ в _HKEY\_LOCAL\_MACHINE\\SOFTWARE\\Microsoft\\Internet Explorer\\Main\\FeatureControl\\FEATURE_BFCACHE_.

2.2. Для 64-битной Windows этот подключ в _HKEY\_LOCAL\_MACHINE\\SOFTWARE\\Wow6432Node\\Microsoft\\Internet Explorer\\Main\\FeatureControl\\FEATURE_BFCACHE_.

3\. Внутри этого подключа создайте параметр с Именем **iexplore.exe**, Типом **REG_DWORD**, Значением **0**.

![create a value named iexplore.exe](../../images/katalon-studio/tutorials/configure_katalon_studio_web_automation_test_project/4.-Katalon-Reg_Dword.png)

Расширение Katalon для Chrome
-----------------------------

Katalon Recorder, [**расширение Katalon**](https://chrome.google.com/webstore/detail/katalon-recorder-selenium/ljdobmomdgdljniojadhoplhkpialdid) для Chrome, требуется для захвата объектов в вашем активном браузере Chrome. Вы можете уставновить расширение Katalon для Chrome [отсюда](https://chrome.google.com/webstore/detail/katalon-recorder-selenium/ljdobmomdgdljniojadhoplhkpialdid). Обратитесь к [Web Object Spy](/x/5BZO) и [Record & Playback](/x/RwnR) за подробностями.

![Katalon Utility](../../images/katalon-studio/tutorials/configure_katalon_studio_web_automation_test_project/5.-Katalon-Addon.png)

Конфигурация портов
-------------------

Эта конфигурация позволяет вам определить какой порт будет использоваться для отправки данных между Katalon Recorder и Katalon Studio.

1. Когда расширение Katalon Recorder добавлено в Chrome, сделайте правый клик на его иконке в правом верхнем углу браузера и откройте **Параметры**, чтобы назначить предпочитаемый порт для обмена данными с Katalon Studio (значение по-умолчанию - 50000).

![open the Options setting](../../images/katalon-studio/tutorials/configure_katalon_studio_web_automation_test_project/6.Katalon-Utility.png)

2\. Откройте настройки Katalon Recorder в Katalon Studio через меню **Window > Preferences > Katalon > Utility Addon**. Введите тот же номер порта, который будет использоваться для обмена данными с Katalon Recorder.

![Katalon Utility Addon](../../images/katalon-studio/tutorials/configure_katalon_studio_web_automation_test_project/7.-Katalon-Utility-Addon.png)

Настройки прокси
----------------

Возможна  ситуация, когда ваш компьютер настроен в ограниченной сети с политикой доступа в Интернет только через прокси сервер. В этом случае настройки прокси могут быть сделаны в **Preferences > Proxy**. Эти настройки влияют на выполнение тестов как через веб-интерфейс, так и на тесты веб-сервисов. (Обратитесь к своему сетевому администратору, чтобы получить информацию об этих настройках).

![Katalon Proxy Settings](../../images/katalon-studio/tutorials/configure_katalon_studio_web_automation_test_project/8.-Katalon-Proxy-Settings.png)

Настройки сертификатов
----------------------

Пользователи могут обнаружить, чтоих компьютеры работают в сети, требующей сертификации для доступа к Интернет.

Katalon Studio поддерживает возможность обхода проверки сертификата, чтобы пользователи с ограниченными сетевыми политиками могли работать с Katalon Studio, как обычно. Эти настройки могут быть найдены в **Project > Settings > Network**. Эти настройки влияют на выполнение тестов как через веб-интерфейс, так и на тесты веб-сервисов.

![Katalon Certificate Settings](../../images/katalon-studio/tutorials/configure_katalon_studio_web_automation_test_project/9.-Katalon-Certificate-settings.png)
