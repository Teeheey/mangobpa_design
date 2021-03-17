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
* Мониторинг бизнес-процессов
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

amocrm.ru, там можно на 14 дней учетку левую создать, если нам потребуется продолжать на них смотреть и копировать, я насоздаю еще  
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



### Меню
---
Мне очень нравится, как выглядит меню в [АМО](amocrm.ru). Слева находится перечень модулей, есть переход на свой профиль. Оставляем как есть
![Amo-like design!](/images/base_amo.png "Amo-lie design")



### Дашборд (первичная страница)
---
Сюда руководитель сможет добавить нужные ему метрики, показатели, события
Особо требований к макету нет, можно пустых блоков (некликабельных) разных размеров добавить, чтобы создать представление, как это буддет выглядеть
Реализовывать будем в последнюю очередь



### Оргстэк
---
Экран должен в себе содержать информацию о том, кто работает в комапнии, в каком отделе и кто у него руководитель  
![image](/images/orgstack.png "image")
Справа вверху должна быть кнопка "+Сотрудник", (в будущем доступна только избранным), клик на которую открывает карточку нового сотрудника  
Справа вверху должна быть кнопка "+Отдел", (в будущем доступна только избранным), клик на которую открывает карточку нового отдела  

###### Карточка нового сотрудника
Карточка должна содержать в себе поля: ФИО, email ( пока-что), должность, должен быть выпадающий список "отдел" в котором будут все созданные отделы  
![image](/images/new_employee.png "image")  
###### Карточка нового отдела
Карточка должна содержать в себе поле название отдела 

Обе карточки должны иметь кнопки "Сохранить" и "Отмена".  Нажатие на которые возвращают на экран Мониторинга бизнес-процессов

Клик на любую запись (сотрудник/отдел) должен открывать ту же карточку сотрудника/отдела



### Мониторинг бизнес-процессов
---
![image](/images/monitoring.png "image")  
Экран представляет из себя разделенный на 2(будет кастомизироваться от  1 до бесконечности) вертикальных блока
Каждый представляет из себя набор записей с "чек-боксами" рядом, блок имеет название сверху
Снизу каждого блока распологается кнопка Сохранить.
По клику на Сохранить:
1) Появляется запись о времени сохранения
2) Все записи с непроставленными галочками подсвечиваются красным (как-то сигнализировать, что что-то не очень хорошо)
Изменять строки нельзя ( это будет настраиваться руководителем )
Слева вверху есть кнопка "HELP", по клику на которую отображается карточка Сообщить о проблеме
###### Карточка сообщения о проблеме
Карточка представляет из себя форму, где можно выбрать из выпадающего списка пунктов, котороые сотрудник должен соблюдать и поля, где можно оставить комментарий, мол "НЕ ВЫПОЛНИМО, ВЫ ЧЕ ТАМ СОВСЕМ ВСЕ"

Карточка имеет кнопки сохранить и отменить. Нажатие на которые возвращают на экран Мониторинга бизнес-процессов



### Мониторинг задач/целей
---
![image](/images/tasks.png "image")  
Экран должен представлять из себя список колонок (по-дефолту - 3) с названиями наверху, и количеством карточек в каждой из них
Карточку (задачу) можно перенести руками из одной колонки в другую, в обе стороны
Справа вверху должна быть кнопка "Создать" клик на которую открывает карточку задачи
Сверху должно располагаться поле фильтрации, в которое можно вводить текст
######  Карточка задачи
Карточка должна отражать суть задачи (ответственный, описание) для начала, представлять из себя аналог задачи в Jira/Amo

Карточка должна иметь кнопки "Сохранить" и "Отмена".  Нажатие на которые возвращают на экран Мониторинга бизнес-процессов



### СРМ
---
![image](/images/crm.png "image")  
Экран должен представлять из себя список колонок (по-дефолту - 3) с названиями наверху, и количеством карточек в каждой из них
Карточку (клиента/сделку) можно перенести руками из одной колонки в другую, в обе стороны
Справа вверху должна быть кнопка "Создать" клик на которую открывает карточку сделки
Сверху должно располагаться поле фильтрации, в которое можно вводить текст
######  Карточка сделки
Карточка должна отражать суть сделки (фио клиента, сумма) для начала, представлять из себя аналог задачи в Jira/Amo

Карточка должна иметь кнопки "Сохранить" и "Отмена".  Нажатие на которые возвращают на экран Мониторинга бизнес-процессов




### ФИН-УЧЕТ
NOT YET DONE

### Ресурсы
NOT YET DONE

### Кастомизация
NOT YET DONE
