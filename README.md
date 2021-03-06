# Задание на создание мокапа системы манго

## Ответы на вопросы Марии 
>  расскажи про компанию проект в целом (это хостел или уже что-то новое?)

Компании еще нет, есть только проект, никак не связанный с гостиницей для кошек.
>  Что это за приложение?

Это приложение, помогающее бизнесменам в организации своего дела.
С помощью нашего приложения бизнесмен сможет:
* обрисовать ожидаемое(требумое) поведение от своих сотрудников, а именно что и когда они должны делать
* описать требования к бизнес-процессам, в каком состоянии должно быть **что-то**, чтобы его бизнес работал (например, у сотрудницы магазина должна быть чековая лента, работать кондей, интернет и чистый пол)

Сотрудник сможет:
* создавать задачи на других сотрудников (исходя из организационных связей)
* не путаться в своих обязанностях а делать все вовремя и "по-расписанию", если требуется

А ТАК ЖЕ:
* система будет отслеживать выполнение/невыполнение задач, неполадки в бизнес-процессах, нарушения(невыполнение) чек-листов сотрудников и создавать **реакции** то есть некоторые действия, помогающие решить проблему
* система будет собирать статистику и аналитику по событиям и давать руководителю(и самым главным дядям) то, что нужно именно им. Уведомлять о том, что нужно именно ом

Остальные модули:
* CRM
* Учет ресурсов (например, если сотрудница сделала маникюр цветом *Цвет_1*, то выполненный заказ будет учитываться на "складе", то есть ресурса *Лак цвет_1* должен будет уменьшиться. Как раз-таки реакция
* Финансовый учет (простой приход/расход) расчитываемый исходя из событий (клиент принес денег - в казне прибавилось, мы заукупили расходники - денег убавилось)
* Оргструктура (связи между сотрудниками и их руководителями, отделы и прочее)
>  какие должны быть экраны (например в соц сети Вк есть экран мессенджер,друзья, профиль, настройки и тд (т.е. это целые страницы)

Основные:
* Задачи
* СРМ
* Чек-листы
* Фин учет
* Орг стэк
* Ресурсы
* Кастомизация

Остальное:
* Профиль
* Лента уведомлений

>  структура (чем лучше пропишешь, тем будет проще и работать) (под ней подразумеваю что должно быть на экранах)

Чуть ниже
>  Примеры. Есть ли на рынке уже что-то подобное, что вам нравится как работает? (будет круто, если вдруг найдешь 2-3 штуки)

[да, конечно](https://amocrm.ru), там можно на 14 дней учетку левую создать, если нам потребуется продолжать на них смотреть и копировать, я насоздаю еще  
мне там нравится расположение, основные модули в ленте слева, события справа вверрху  
да и вообще, СРМ и задачи будем делать примерно так же  


## Ожидание от дизайнера
(будем называть его/ее так)  
Хочется увидеть что-то, где будущий клиент (и мы) сможем кликать на кнопки, желательно таскать карточки и видеть, что экраны меняются, что-то появляется, что-то нет  
Оформление - не так важно, в каком-то одном цвете можно сделать, хоть в черно-белом, бренд-бука нет. Но должны быть соблюдены требования к переходам.  
Важно показать, что будет происходить если, и что не будет происходить не если  
*У нас нет требования нарисовать красивый дизайн, есть только желание создать клибаельный макет чтобы мочь презентовать будущий продукт*  


## ПАЕХАЛИ
*Я опишу сейчас не все, а только первые несколько модулей, которые мы активно прорабатываем, если у тебя(дизайнер) не будет чем заняться - подумаем над дальнейшим*  
**Bсе картинки, которые я приложил - приложены лишь для общего представления, что мы хотим видеть, это не является прямым указанием, все, кроме мониторинга бизнес-процессов брал из интернетов, поэтому и дизайн разный**  



### Меню
---
Мне очень нравится, как выглядит меню в [АМО](amocrm.ru). Слева находится перечень модулей, есть переход на свой профиль. Оставляем как есть
![Amo-like design!](/images/base_amo.png "Amo-lie design")



### Дашборд (первичная страница)
---
Сюда можно добавить нужные ему метрики, показатели, события
Особо требований к макету нет, можно пустых блоков (некликабельных) разных размеров добавить, чтобы создать представление, как это буддет выглядеть
Реализовывать будем в последнюю очередь



### Оргстэк
---
Экран должен в себе содержать информацию о том, кто работает в комапнии, в каком отделе и кто у него руководитель  
![image](/images/orgstack.png "image")  
Справа вверху должна быть кнопка "+Сотрудник", (в будущем доступна только избранным), клик на которую открывает карточку нового сотрудника  
Справа вверху должна быть кнопка "+Отдел", (в будущем доступна только избранным), клик на которую открывает карточку нового отдела  
Справа вверху должна быть кнопка "+Должность", (в будущем доступна только избранным), клик на которую открывает карточку новой должности

###### Карточка нового сотрудника
Карточка должна содержать в себе поля: ФИО, email ( пока-что), выпадающий список должность, выпадающий список "отдел"  
![image](/images/add_employee.png "image")  

###### Карточка нового отдела
Карточка должна содержать в себе поле название отдела 

###### Карточка новой должности
Карточка должна содержать в себе поле название должности

Обе карточки должны иметь кнопки "Сохранить" и "Отмена".  Нажатие на которые возвращают на экран огрстэкa

Клик на любую запись (сотрудник/отдел) должен открывать ту же карточку сотрудника/отдела



### Чек-листы
---

Экран представляет из себя разделенное на 2 вкладки(Текущие/Завершенные) с списком чек-листов
Каждая вклада содержит набор блоков со строками и "чек-боксами" рядом, блок имеет название сверху

> Вкладка текущие
![image](/images/check-list_current.png "image")  

Актуальный ( будет определяться по текущему времени ) блок - раскрыт  
Предстоящие - свернуты  
Снизу текущего блока распологается кнопка Сохранить.  
По клику на Сохранить:  
1) Появляется запись о времени сохранения  
2) Все записи с непроставленными галочками подсвечиваются красным (как-то сигнализировать, что что-то не очень хорошо)  
3) Блок переносится на вкладку "Завершенные"  

> Вкладка завершенные
![image](/images/check-list_finished.png "image")  

Все блоки свернутые  
По клику на блок - раскрывается  
Невыполненные записи подсвечиваются красным  


Справа вверху есть кнопка "Претензии к чек-листу", по клику на которую отображается карточка "Претензии к чек-листу"  
Справа вверху есть кнопка "Сообщить о проблеме", по клику на которую отображается карточка Сообщения о проблеме  

###### Карточка Претензии к чек-листу
Карточка представляет из себя форму, где можно выбрать из выпадающего списка один из пунктов, котороые сотрудник должен соблюдать и поля, где можно оставить комментарий, касательно этого пункта. Например, сообщить руководителю о том, что какой-то пункт невыполним

###### Карточка Сообщить о проблеме
Карточка представляет из себя форму, где можно сообщить о какой-то проблеме, нарушающей текущее состояние бизнес-процесса

Карточки имеют кнопки сохранить и отменить. Нажатие на которые возвращают на экран Чек-листов

  
    



### Задачи
---
![image](/images/tasks.png "image")  
Экран должен представлять из себя список колонок (по-дефолту - 3) с названиями наверху, и количеством карточек в каждой из них
Карточку (задачу) можно перенести руками из одной колонки в другую, в обе стороны
Справа вверху должна быть кнопка "Создать" клик на которую открывает карточку задачи
Сверху должно располагаться поле фильтрации, в которое можно вводить текст
######  Карточка задачи
Карточка должна отражать суть задачи (ответственный, описание) для начала, представлять из себя аналог задачи в Jira/Amo

Карточка должна иметь кнопки "Сохранить" и "Отмена".  Нажатие на которые возвращают на экран Задачи




### СРМ
---
![image](/images/crm.png "image")  
Экран должен представлять из себя список колонок (по-дефолту - 3) с названиями наверху, и количеством карточек в каждой из них
Карточку (клиента/сделку) можно перенести руками из одной колонки в другую, в обе стороны
Справа вверху должна быть кнопка "Создать" клик на которую открывает карточку сделки
Сверху должно располагаться поле фильтрации, в которое можно вводить текст

######  Карточка сделки
Карточка должна отражать суть сделки (фио клиента, сумма) для начала, представлять из себя аналог задачи в Jira/Amo

Карточка должна иметь кнопки "Сохранить" и "Отмена".  Нажатие на которые возвращают на экран CRM



### TODO

> ФИН-УЧЕТ  

> Ресурсы  

> Кастомизация  

> Цели
