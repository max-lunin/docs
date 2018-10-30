---
title: "Установка и настройка Katalon Studio"
sidebar: katalon_studio_tutorials_sidebar
permalink: katalon-studio/tutorials/install_setup_katalon_studio.html
description: "Это руководство является кратким введением к Katalon Studio, от загрузки до активации и запуска вашего первого автотеста."
---
Katalon Studio это простое и мощное решение для автоматизации тестирования не только мобильных и веб-приложений, но и веб-сервисов, — революция фреймворков Selenium и Appium. Katalon Studio позволяет пользователям с небольшим опытом в программировании работать без усилий, предоставляя автоматизационный фреймворк с сотнями встроенных ключевых слов. В этом руководстве объясняются все основные этапы, от загрузки до активации приложения, так что новые пользователи могут впервые запустить Katalon Studio.

Загрузка Katalon Studio
-----------------------

Katalon Studio бесплатен, поддерживаются версии как для Windows, так и для Mac. Посетите [вебсайт Katalon Studio](https://www.katalon.com/) чтобы загрузить последнюю версию.

Конфигурация окружения
----------------------

Сначала вам необходимо проверить, соответствует ли ваш компьютер [Системным требованиям](http://docs.katalon.com/display/KD/System+Requirements) для выполнения автоматизации, используя Katalon Studio.

Для **Web UI**-автоматизации, дополнительных настроек не требуется, кроме установленных необходимых браузеров. Проверьте [этот список](/x/dAAM) поддерживаемых браузеров.

Обратите внимание: в случае если вы - пользователь Windows, вы можете захотеть отключить **User Access Control (UAC)**, чтобы Katalon Studio мог запускать браузеры Chrome/Firefox правильно. Обратитесь к [этому руководству](https://www.howtogeek.com/howto/windows-vista/disable-user-account-control-uac-the-easy-way-on-windows-vista/) за необходимыми действиями по отключению UAC на разных версиях Windows.

Для автоматизации **мобильных** приложений, вам необходимо установить **Node.js** и **Appium** и активировать режим **USB Debugging mode** на вашем устройстве. Пожалуйста обратитесь к [руководству по установке](http://docs.katalon.com/display/KD/Installation+and+Setup) за подробностями.

Запуск Katalon Studio
----------------------

Чтобы запустить Katalon Studio, сделайте двойной щелчок на файле **katalon.exe** (Microsoft Windows)

![Download and Start Katalon Studio](../../images/katalon-studio/tutorials/install_setup_katalon_studio/Starting-Katalon-Studio.png)

или файле **Katalon Studio** (macOS) в директории, в которую вы распаковали Katalon Studio. Например:

![](../../images/katalon-studio/tutorials/install_setup_katalon_studio/Katalon-MacOS.png "init-size")

После запуска приложение должно отобразить заставку как на следующем скриншоте:

![Katalon Studio Loading](../../images/katalon-studio/tutorials/install_setup_katalon_studio/image2016-10-20-143A113A21.png)

Активация Katalon Studio
------------------------

После запуска Katalon Studio введите имя пользователя и пароль, чтобы активировать ваш Katalon Studio. Имя пользователя и пароль те же, что вы использовали при регистрации чтобы загрузить Katalon Studio с [https://www.katalon.com/](https://www.katalon.com/).

![Katalon Studio Activation pop-up](../../images/katalon-studio/tutorials/install_setup_katalon_studio/image2017-2-16-173A303A12.png)

Если у вас сложности с активацией Katalon Studio из-за прокси, вы можете нажать на [Config Proxy](/display/KD/Proxy+Preferences), чтобы сконфигурировать прокси соответствующим образом.

Если вы не можете получить доступ к Интернет для активации, вы можете выбрать **Offline Activation** чтобы активировать Katalon Studio офлайн. Вам необходимо запросить активационный код [здесь](https://www.katalon.com/activation/).

Когда ваше приложение активировано отображается экран **Quick Guide**, который познакомит вас со всеми основными функциями. Вы можете его пропустить и просмотреть позже, вызвав Quick Guide из меню **Help**.

![Katalon Studio Quick Guide Overview](../../images/katalon-studio/tutorials/install_setup_katalon_studio/image2017-2-20-113A303A20.png)

Вы успешноскачали и активировали Katalon Studio. Далее пожалуйста обратитесь к следующим руководствам, чтобы настроить ваш тестовый проект:

*   [Настройка проекта автоматизации Веб-тестирования](/katalon-studio/tutorials/get-started/kickstart-automation-testing-using-katalon-studio/)
*   [Настройка проекта автоматизации мобильного тестирования в Windows](/katalon-studio/tutorials/get-started/set-up-mobile-automation-project-windows/)
*   [Настройка проекта автоматизации мобильного тестирования в macOS](/katalon-studio/tutorials/get-started/set-up-mobile-automation-project-macos/)
*   [Настройка проекта автоматизации тестирования API](/katalon-studio/tutorials/get-started/set-up-api-testing-project/)
