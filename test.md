# Основные команды Git

**Git init** - инициализация локального репозитория.

**Git add** - добавили файл для отслеживания изменений в нём или файлы к следующему коммиту.

**Git add --all**  или **Git add .** - добавить все файлы в репозитории к отслеживанию изменений. 

**Git commit -m "текст сообщения"** - создание коммита *(т.е. фиксация изменения, сделан снимок файла, создана его новая версия и приложено сообщение к нему)*.

**Git commit -a -m "текст сообщения"** - так кратко записываются 2 предидущие команды в одну команду, add + commit одновременно.

**Git status** - получить информацию о текущем состоянии файлов в репозитории.

**Git log** - вывод на экран истории всех коммитов (версий) с их хеш-кодами (адресами).


**Git diff** - увидеть разницу между текущим файлом и закоммиченным файлом.

*(P.S. При этом текущий файл должен быть сохранен, только тогда эти изменения будут отмечены зеленым цветом после команды git diff.)*.

**Git branch** - увидеть список веток в репозитории.

**Git branch** *и далее имя новой ветки* - создать новую ветку с указанным именем, имя новой ветки указываем после команды.

**Git branch -d** *и далее имя удаляемой ветки* - удаление ветки, имя ветки указываем после команды.

**Git log --graph** - увидеть лог комитов, графически ветки изменений.

**Git checkout** *и далее имя*- переход от одного коммита (файла) или ветки к другому (надо добавить после команды имя файла или имя ветки куда надо переместиться).

**Git checkout master** - вернуться к актуальному состоянию и продолжить работу.

**Git checkout -b** *и далее имя новой ветки* - создаем новую ветку и сразу переходим на неё, объединяет 2 команды в одну.

**Git merge** *и далее имя ветки для слияния с текущей* - слияние веток, надо встать на ветку к которой сливаем, и после команды указать имя присоединяемой ветки.

## Добавление изображений

Делаем так: перемещаем в репозиторий фото, при этом в названии файла не должно быть пробелов, далее используем знак и две пары скобок ![сюда пишем сообщение на случай ошибки](сюда имя загружаемого файла). И получем изображение фото или картинки.

![добавляю фото](Riga2.jpeg)

В Git не храним файлы с изображениями, их хранят на сторонних носителях. Чтобы исключить сторонние файлы из загрузки их перемещаем в созданный файл для игнорирования того, что туда поместим, файл называем:

**.Gitignore**

После в созданный файл .gitignore добавляем сторонние файлы для их игнорирования.

## Ссылки

Делаем так: используем знак и две пары скобок ![сюда пишем описание ссылки, типа заголовка для ссылки](сюда путь к файлу из интернета или иного источника). И получем ссылку на сайт или на файл.

! [Значение ключевой ставки ЦБР смотри здесь](https://cbr.ru)


## Цитаты

Делаем так: используем знак >

> [Значение ключевой ставки ЦБР смотри здесь](https://cbr.ru)

> В Git не храним файлы с изображениями, их хранят на сторонних носителях. Чтобы исключить сторонние файлы из загрузки их перемещаем в созданный файл для игнорирования того, что туда поместим, файл называем:

Обычно блок цитирования отображается с отступом и имеет другой цвет фона.

## На этом ДЗ1 к семинару 1 закончено.


# Домашнее задание № 2. Работа с ветками.

## Задача: сделать краткий анализ по двум акциям из нефтегазовой отрасли и двум акциям из металлургической отрасли.

### Каждого эмитента рассмотрим на своей ветке.

### Сравним динамику каждой акции с динамикой индекса МосБиржи начиная с 2020 года и определим силу или слабость каждой акции.


![Индекс МосБиржы](mbindex2.png)


### Между двумя бумагами из одной отрасли создадим конфликт.

#### Нефтегазовая отрасль

* Газпромнефть

Нефтяная компания, бывшая Сибнефть. 
Платит дивиденды 2 раза в год, ближайшие планируются по итогам 9 месяцев 2023 года, ожидаем 50-52 рубля на акцию.
Бумага уже превысила свой уровень до начала СВО и свой исторический максимум.
Коррекция в сентябре не значительная.
Бумага одна из самых сильных на рынке. 

График цены по акциям Газпромнефти с 2020 года ниже:

![Газпромнефть](sibn23.PNG)

* Газпром

Планирую покупать акции Газпрома только при его коррекции до уровня 150 рублей.  Бумага слабая, дивиденды под вопросом.

Газовый монополист на рынке поставок трубопроводного газа в ЕС. В связи с СВО и взрывом трубопровода *Северный поток* полностью потерял рынок ЕС.
В июне 2022 года отказал в выплате утвержденных ранее на СД дивидендов, чем уронил свои акции в 2 раза. С тех пор цена колеблется на своих минимумах, что были при короновирусе и при начале СВО.
Бумага слабая, даже при коррекции снижение не значительное, фундаментальных причин для роста пока нет.

График акций Газпром с 2020 года ниже:

![график по акциям Газпром](gazprom23.PNG)

#### Металлургия

* ММК

Магнитогорский металлургический комбинат, предприятие черной металлургии. Работает в основном на рынок РФ и стран СНГ. Попал под санкции в июле 2022 года в связи с чем акции обвалились до 23 рублей.

Дивиденды прекратил выплачивать с 2022 года, ждем их возобновления по итогам 2023 года.
Бумага средняя по силе, планирую покупать на осенней коррекции на уровне 45-47 рублей.

График по акциям ММК ниже:

![график по акциям ММК](magn23.PNG)
Вывод: акции ММК самые ликвидные среди акций черных металлургов, данная бумага наиболее желательна в портфеле.

* НЛМК

Новолипецкий металлургический комбинат. Предприятие черной металлургии. На 70% работает на экспорт в основной части в Китай. 

Прекратил выплату дивидендов в 2022 году, возможное восстановление выплат по итогам 2023 года.

Бумага средняя по силе, см. график ниже:

![график по акциям нлмк](nlmk23.PNG)



## Семинар № 3

**Создал новый репозиторий на GitHub назвал его Seminar3**

Из локального репозитория командой push поместил в него ДЗ №2

Вернулся на свой ноут и создал на нем папку Seminar33 и командой pull стянул с GitHub файл ДЗ №2.

Внес в файл изменения и закомитил версию.

Отправил push на GitHub.

