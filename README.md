# OOP
Макаревич Дарья гр. 253505

Разработка приложения «Менеджер финансов».
Данное приложение позволяет пользователю вести учет своих доходов и расходов по категориям, а также составлять статистику расходов. 
Для разработки приложения был выбран язык C#, фреймворк MAUI и язык разметки XAML.

Функциональность:
- Регистрация аккаунта пользователя
- Вход в аккаунт пользователя
- Внесение доходов: добавление денежной суммы к числу доходов, добавление текстового примечания.
- Внесение расходов: добавление денежной суммы к числу расходов по категориям. Виды категорий: продукты, транспорт, одежда, здоровье, коммунальные счета, развлечения, питомцы, дом, другое. Добавление текстового примечания.
- Показ текущего баланса.
- Генерация статистики и построение диаграммы расходов по категориям с учетом временного интервала (день, неделя, месяц, год, все время, свой временной промежуток).

Используемые классы:
- User - класс, представляющий пользователя. Включает в себя атрибуты, такие как имя пользователя, пароль и логин. Реализует методы: регистрация пользователя, авторизация пользователя. 
- ExpenseTracker - основной класс, отвечающий за отслеживание расходов и доходов. В нем будут храниться списки доходов и расходов, а также реализованы методы для добавления доходов, расходов и расчета баланса.
- Income - класс, представляющий доход. Содержит атрибуты для хранения суммы дохода, текстового примечания и даты.
- Expense - класс, представляющий расход. Включает в себя атрибуты для суммы расхода, категории (продукты, транспорт и т. д.), текстового примечания и даты.
- StatisticGenerator - класс для генерации статистики и построения диаграммы расходов по категориям с учетом временного интервала. Он будет содержать методы для анализа данных о расходах, а также методы для построения диаграммы.
- DataBase – класс для работы с базой данных. Он будет содержать атрибуты для хранения объекта подключения к БД, объект БД. А также методы для подключения, чтения, обновления, удаления и записи данных в БД.

Столбцы в БД: Состояние (доход/расход), сумма, категория, дата, пользователь.

