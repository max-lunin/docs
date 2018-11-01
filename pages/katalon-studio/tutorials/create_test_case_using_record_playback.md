---
title: "Создание тест-кейса, используя Запись и Воспроизведение"
sidebar: katalon_studio_tutorials_sidebar
permalink: katalon-studio/tutorials/create_test_case_using_record_playback.html
redirect_from:
  - "/katalon-studio/tutorials/sample_web_automation_test_project.html"
description: "Запись теста - это самый легкий путь для новичка начать изучение автоматизации тестирования. Эта статья показывает как легко записать тест-кейс."
---
Запись теста - это самый легкий путь для новичка начать изучение автоматизации тестирования. Идентификация объектов приложения - трудоемка и болезненна. [Web Recorder](http://docs.katalon.com/pages/viewpage.action?pageId=5118055) захватывает ваши действия, выполняемые над приложением, и конвертирует их в исполняемый код в бек-энде. Используя это, вы можете быстро автоматизировать несколько функций вашего приложения и сэкономить время, записывая действия, которые нужно выполнять довольно много раз в итерационных сборках. Эта фукнкция Katalon Studio поддерживает запись и запуск одних и тех же тестов в разных браузерах. Эта статья показывает как легко записать тест-кейс.

1.  [Запись вашего первого теста с помощью функции Katalon Studio "Record Web"](#record-first-test)
2.  [Как изменить имя папки страницы и имена элементов во время записи](#change-page-folder-names)
3.  [Как добавить команды Katalon во время записи](#add-katalon-commands)

Запись вашего первого теста с помощью функции Katalon Studio "Record Web"
-------------------------------------------------------------------------

**Сценарий:** Создать запись на прием

1.  Запустите тестируемое приложение (**URL**: [http://demoaut.katalon.com/](http://demoaut.katalon.com/))
2.  Нажмите кнопку "Make Appointment"
3.  Введите действительные имя пользователя и пароль, нажмите на кнопку "Login"
4.  Создайте запись на прием

Следуйте нижеприведенным шагам, чтобы познакомиться с функцией записи и воспроизведения теста вебинтерфейса.

**Шаг 1:** Запустите Katalon Studio и нажмите **New > Test Case** на главной панели инструментов. Введите название вашего тест-кейса и нажмите кнопку **OK**. Будет создан пустой тест-кейс.

![Создание тест-кейса](../../images/katalon-studio/tutorials/create_test_case_using_record_playback/Create-Test-Case.png)

**Шаг 2:** Нажмите кнопку **Record Web** на главной панели инструментов.

![Record-Web](../../images/katalon-studio/tutorials/create_test_case_using_record_playback/Record-Web.png)

**Шаг 3:** Отобразится диалоговое окно **Web Recorder**.

![Web recorder](../../images/katalon-studio/tutorials/create_test_case_using_record_playback/Record-Dialog-300x254.png)

**Шаг 4:** Выберите браузер и нажмите кнопку **Record** чтобы начать запись тест-кейса.

![запись тест-кейса](../../images/katalon-studio/tutorials/create_test_case_using_record_playback/recording-test-case.png)

**Шаг 5:** Когда приложение будет запущено наведите курсор на кнопку **'Make Appointment'** и нажмите на нее (подождите пока загрузится страница аутентификации).

![Создание записи на прием](../../images/katalon-studio/tutorials/create_test_case_using_record_playback/Make-Appointment-e1513053243772-1024x512.png)

**Шаг 6:** Введите действительные имя пользователя и пароль (John Doe и ThisIsNotAPassword), нажмите на кнопку "Login" (подождите пока страница загрузится).

![Аутентификация для создания записи](../../images/katalon-studio/tutorials/create_test_case_using_record_playback/Login-to-Make-Appointment-e1513053339776.png)

**Шаг 7:** Когда страница создания записи загрузится, выберите **"Hongkong CURA Healthcare Center"** из выпадающего списка "Facility".

![Страница создания записи](../../images/katalon-studio/tutorials/create_test_case_using_record_playback/Make-Appointment-page-e1513067371591.png)

**Шаг 8:** Наведите курсор на чекбокс '**Apply for hospital readmission**' и кликните на нем.

**Шаг 9:** Переместите курсор к радио-кнопкам и кликните на кнопке **'Medicaid'.**

**Шаг 10:** Кликните на иконке календаря в поле '**Visit Date'** и кликните на необходимой дате.

![Календарь](../../images/katalon-studio/tutorials/create_test_case_using_record_playback/Calendar-e1513067438109.png)

**Шаг 11:** Поместите курсор в поле "Comment"и введите текст.

**Шаг 12:** Наведите курсор на кнопку **Book Appointment** и нажмите на нее.

**Шаг 13:** Вы можете остановить запись в любой момент, нажав на кнопку '**Stop**'. Katalon Studio позволяет пользователям выбрать метод определения захватываемых объектов. **Basic mode** рекомендуется для ручных тестировщиков, которые только начинают осваивать автоматизацию. В базовом режиме интеллектуальный генератор селекторов Katalon Studio будет **автоматически генерировать** надежные и уникальные **селекторы** для захватываемых объектов.

Для опытных тестировщиков, которые хотят **вводить селекторы вручную** есть выбор между **CSS** и **XPath mode**. За подробностями о методах определения захватываемых объектов обратитесь к этому [руководству](http://docs.katalon.com/pages/viewpage.action?pageId=5118311).

![Katalon Web Recorder](../../images/katalon-studio/tutorials/create_test_case_using_record_playback/Selection-Method-for-captured-objects.png)

**Шаг 14:** Когда вы закончили запись, нажмите кнопку **OK**, чтобы сохранить записанные действия в Katalon Studio. Вам будет предложено сохранить захваченные объекты в **Object Repository** который при необходимости может быть использован повторно**.** Вы также можете создать папку, чтобы хранить и обслуживать объекты страницы в желаемом порядке. Нажмите кнопку **OK** чтобы продолжить**.**

![Object-Repository](../../images/katalon-studio/tutorials/create_test_case_using_record_playback/Object-Repository.png)

**Шаг 15:** Записанные объекты и действия сохранены в тест-кейс, как показано ниже.

![Записанные объекты](../../images/katalon-studio/tutorials/create_test_case_using_record_playback/Recorded-objects-e1513067504997.png)

Просто нажмите кнопку **'Run'**, чтобы запустить записанный тест-кейс в желаемом браузере.

**Код скрипта записи и воспроизведения**

```groovy
WebUI.openBrowser('')
WebUI.navigateToUrl('http://demoaut.katalon.com/')</p>
WebUI.click(findTestObject('Page_CURA Healthcare Service/a_Make Appointment'))
 
WebUI.click(findTestObject('Page_CURA Healthcare Service (1)/button_Login'))
 
WebUI.selectOptionByValue(findTestObject('Page_CURA Healthcare Service (2)/select_facility'), 'Hongkong CURA Healthcare Center',
 
true)
 
WebUI.click(findTestObject('Page_CURA Healthcare Service (2)/input_hospital_readmission'))
 
WebUI.click(findTestObject('Page_CURA Healthcare Service (2)/input_programs'))
 
WebUI.click(findTestObject('Page_CURA Healthcare Service (2)/div_input-group-addon'))
 
WebUI.click(findTestObject('Page_CURA Healthcare Service (2)/td_3'))
 
WebUI.setText(findTestObject('Page_CURA Healthcare Service (2)/textarea_comment'), 'Katalon')
 
WebUI.click(findTestObject('Page_CURA Healthcare Service (2)/button_Book Appointment'))
 
WebUI.closeBrowser()

```

Как изменить имя папки страницы и имена элементов во время записи
-----------------------------------------------------------------

Для организации тестовых скриптов по шаблону объекта страницы, необходимо добавить тестовые объекты в папку, соответствующую странице. Это помогает при повторном использовании объекта и обслуживании объектов.

**Сценарий:** Аутентификация с действительными данными

1.  Запустите тестируемое приложение (**URL**: [http://demoaut.katalon.com/](http://demoaut.katalon.com/)).
2.  Нажмите на кнопку "Make Appointment" (измените имена страницы и элемента).
3.  Введите действительные имя пользователя и пароль, нажмите на кнопку "Login" (измените имена страницы и элемента).

**Шаг 1:** Запустите Katalon Studio и нажмите кнопку **First Test Case** на главной панели инструметов. Введите название вашего тесткейса и нажмите кнопку **OK**. Будет создан пустой тест-кейс.

![Изменение имени элемента](../../images/katalon-studio/tutorials/create_test_case_using_record_playback/Change-Element-Name.png)

**Шаг 2:** Нажминте на **Record Web** на главной панели инструметов.

![Record-Web](../../images/katalon-studio/tutorials/create_test_case_using_record_playback/Record-Web.png)

**Шаг 3:** Отобразится диалоговое окно **Record**. Выберите браузер и нажмите кнопку **Record** чтобы начать запись тест-кейса.

![запись тест-кейса](../../images/katalon-studio/tutorials/create_test_case_using_record_playback/recording-test-case.png)

**Шаг 4:** Когда приложение будет запущено наведите курсор на кнопку **'Make Appointment'** и нажмите на нее (подождите пока загрузится страница аутентификации).

![Диалоговое окно записи](../../images/katalon-studio/tutorials/create_test_case_using_record_playback/Record-Dialog-Box.png)

**Step 5:** Переименуйте страницу с **"Page_CURA Healthcare Service"** на **"Page_Home Page".**

**Шаг 6:** Выберите элемент **"a_Make Appointment"** в поле "Captured Objects".

**Шаг 7:** Переименуйте элемент с **"a_Make Appointment"** на **"button_Make Appointment".**

![Web-Recorder-Utility](../../images/katalon-studio/tutorials/create_test_case_using_record_playback/Web-Recorder-Utility.jpg)

**Шаг 8:** Затем продолжайте запись, для чего переключитесь на записываемый браузер, наведите курсор на кнопку **Login** и нажмите на нее**.**

![Аутентификация для создания записи](../../images/katalon-studio/tutorials/create_test_case_using_record_playback/Login-to-Make-Appointment-e1513053339776.png)

**Шаг 9:** Повторите шаги, приведенные выше, чтобы переименовать объект **Login** и его папку.

**Шаг 10:** Переименуйте страницу с **"Page_CURA Healthcare Service"** на **"Page_Login".**

![Web-Recorder-Utility-2](../../images/katalon-studio/tutorials/create_test_case_using_record_playback/Web-Recorder-Utility-2.jpg)

**Шаг 11:** Вы можете остановить запись в любой момент, нажав на кнопку '**Stop**'. Когда вы закончили запись, нажмите кнопку **OK**, чтобы сохранить записанные действия в Katalon Studio. 

**Шаг 12:** Вам будет предложено сохранить захваченные объекты в **Object Repository** который при необходимости может быть использован повторно**.** Вы также можете создать папку, чтобы хранить и обслуживать объекты страницы в желаемом порядке. Для продолжения нажмите кнопку **OK**.
![Objects-repository](../../images/katalon-studio/tutorials/create_test_case_using_record_playback/Objects-repository.png)

**Шаг 13:** Записанные объекты и действия сохранены в тест-кейс, как показано ниже..

![Записанные объекты и действия-2](../../images/katalon-studio/tutorials/create_test_case_using_record_playback/Recorded-objects-and-actions-e1513069057639.png)

Просто нажмите кнопку **'Run'**, чтобы запустить записанный тест-кейс в желаемом браузере.

**Исходный код:**

```groovy
import static com.kms.katalon.core.testobject.ObjectRepository.findTestObject</p>
import com.kms.katalon.core.webui.keyword.WebUiBuiltInKeywords as WebUI
 
WebUI.openBrowser('')
 
WebUI.navigateToUrl('http://demoaut.katalon.com/')
 
WebUI.click(findTestObject('Page_Home Page/button_Make Appointment'))
 
WebUI.click(findTestObject('Page_Login/button_Login'))
 
WebUI.closeBrowser()

```

Как добавить команды Katalon во время записи
--------------------------------------------

**Сценарий:** Проверка аутентификации с валидацией

1.  Запустите тестируемое приложение (url: http://demoaut.katalon.com/)
2.  Проверьте наличие кнопки "Make Appointment"
3.  Нажмите на кнопку "Make Appointment"
4.  Проверьте видимость кнопки "Login"
5.  Введите действительные имя пользователя и пароль, нажмите на кнопку "Login"

Во время записи Katalon Studio позволяет пользователям добавлять дополнительные команды, такие как команды основных действий, команды проверки, команды синхронизации.

**Шаг 1:** Запустите Katalon Studio и нажмите кнопку **New Test Case** на главной панели инструметов. Введите название вашего тесткейса и нажмите кнопку **OK**. Будет создан пустой тест-кейс.

![Создание тест-кейса](../../images/katalon-studio/tutorials/create_test_case_using_record_playback/Create-Test-Case.png)

**Шаг 2:** Нажминте на **Record Web** на главной панели инструметов.

![Record-Web](../../images/katalon-studio/tutorials/create_test_case_using_record_playback/Record-Web.png)

**Шаг 3:** Отобразится диалоговое окно **Record**. 

**![Диалоговое окно Record](../../images/katalon-studio/tutorials/create_test_case_using_record_playback/Record-Dialog.png) **

**Шаг 4:** Выберите браузер и нажмите кнопку **Record** чтобы начать запись тест-кейса.

![Запись тест-кейса](../../images/katalon-studio/tutorials/create_test_case_using_record_playback/recording-test-case.png)

**Шаг 5:** Когда приложение будет запущено наведите курсор на кнопку **'Make Appointment'** и нажмите на нее (подождите пока загрузится страница аутентификации).

![Создание записи](../../images/katalon-studio/tutorials/create_test_case_using_record_playback/Make-Appointment-e1513053243772.png)

**Ifu 6:** Мы можем добавить команды проверки во время записи, для этого нужно переключиться на окно **Katalon record dialog** и нажать кнопку **Add** перед чем необходимо выбрать шаг, после которого будет добавлена строка **команд проверки**.

![Katalon-Record-Dialog](../../images/katalon-studio/tutorials/create_test_case_using_record_playback/Katalon-Record-Dialog.png)

**Шаг 7:** Нажмите на кнопку **Add**.

**Шаг 8:** Это добавит команду по-умолчанию **Accept Alert**, справа от которой располагается маркер выпадающего списка. Нажмите на маркер и выберите из списка **Verify Element Present**. Команде необходимо передать объект, для этого сделайте двойной щелчок в столбце **Object**. Откроется окно **Captured objects**, в котором нужно выбрать **button_Make Appointmen** и нажать кнопку **OK**.

![Verify-Element-Present](http://prntscr.com/ld441c)

**Шаг 9:** Необходимо дать время для проверки наличия элемента **"Verify Element Present"**. Время задержки по-умолчанию - 0 секунд. Чтобы его изменить сделайте двойной щелчок в столбце **Input** и в открывшемся окне **Input** для параметра **timeOut** введите значение **Value** по вашему желанию и нажмите кнопку **OK**.

![Set-timeOut-Value](http://prntscr.com/ld4gij)

**Шаг 10:** В окне **Web Recorder** отобразится команда **Verify Element Present** с **Object = button_Make Appointmen** и **Input** с выбранным значением.

**Шаг 11:** Затем продолжайте запись, для чего переключитесь на записываемый браузер, наведите курсор на кнопку **Make Appointment** и нажмите на нее.

![Login-to-Make-Appointment](../../images/katalon-studio/tutorials/create_test_case_using_record_playback/Login-to-Make-Appointment-e1513053339776.png)

**Шаг 12:** Необходимо добавить проверку для кнопки **Login** для чего переключитесь на окно **Web Recorder**.

**Шаг 13:** Нажмите на кнопку **Add**. 

**Шаг 14:** Это добавит команду по-умолчанию **Accept Alert**.

**Шаг 15:** Теперь необходимо изменить **Accept Alert** на **Verify Element Visible**. Нажмите на маркер выпадающего списка и выберите **Verify Element Visible**. 

![Verify-Element-Visible](../../images/katalon-studio/tutorials/create_test_case_using_record_playback/Verify-Element-Visible.png)

**Шаг 16:** В окне **Web Recorder** будет отображена команда **Verify Element Visible**. 

**Шаг 17:** Команде **Verify Element Visible** необходимо передать объект. Для этого сделайте двойной щелчок в столбце **Object**. Откроется окно **Captured objects**, в котором нужно выбрать **button_Login** и нажать кнопку **OK**.

**Шаг 18:** Команда **Verify Element Visible** будет отображена с модифицированным объектом.

**Шаг 19:** Вы можете остановить запись в любой момент, нажав на кнопку '**Stop**'. Когда вы закончили запись, нажмите кнопку **OK**, чтобы сохранить записанные действия в Katalon Studio. 

![recorded-actions](../../images/katalon-studio/tutorials/create_test_case_using_record_playback/recorded-actions.png)

**Шаг 20:** Вам будет предложено сохранить захваченные объекты в **Object Repository** который при необходимости может быть использован повторно**.** Вы также можете создать папку, чтобы хранить и обслуживать объекты страницы в желаемом порядке. Для продолжения нажмите кнопку **OK**.

**Шаг 21:** Записанные объекты и действия сохранены в тест-кейс, как показано ниже..

![Записанные объекты и действия-3](../../images/katalon-studio/tutorials/create_test_case_using_record_playback/Recorded-objects-and-actions-3-e1513069217546.png)

**Исходный код:**

```groovy
WebUI.openBrowser('')</p>
WebUI.navigateToUrl('http://demoaut.katalon.com/')
 
WebUI.verifyElementPresent(findTestObject('Page_CURA Healthcare Service/a_Make Appointment'), 30)
 
WebUI.click(findTestObject('Page_CURA Healthcare Service/a_Make Appointment'))
 
WebUI.verifyElementVisible(findTestObject('Page_CURA Healthcare Service (1)/button_Login'))
 
WebUI.click(findTestObject('Page_CURA Healthcare Service (1)/button_Login'))
 
WebUI.closeBrowser()

```

Итак, мы можем записывать выполняемые действия с помощью Katalon Studio. Существует несколько действий, которые не могут быть записаны.

### Что не может быть записано?

Хотя запись тестов экономит время, мы не можем проверять несколько сценариев, таких как обработка веб-таблиц, переключение между фреймами, переключение окон, обработку капчей, распознавание изображений, воспроизведение видео. Вот основные недостатки: 

a) Используя рекордер мы не можем обрабатывать динамически изменяющиеся элементы (поскольку нам нужно настроить Xpath / CSS)

b) Мы не можем использовать код повторно когда необходимо. И это довольно сложно для отладки.

Вы можете скачать исходный код [здесь](https://github.com/katalon-studio/katalon-web-automation).

За дальнейшими инструкциями и помощью обратитесь к урокам [Запись тестов вебинтерфейса](/x/RwnR) и [Запись и воспроизведение](https://www.katalon.com/videos/tutorial-videos/create-test-case-record-playback/).
