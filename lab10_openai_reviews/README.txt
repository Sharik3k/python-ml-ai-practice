Практичне заняття 10. OpenAI API

У цій роботі я зробив аналіз відгуків клієнтів через OpenAI API.
Спочатку я завантажив файл reviews.csv, де були відгуки про ресторан.
Потім для кожного відгуку модель визначила настрій, теми і пропозиції для покращення.

Кількість відгуків: 50

Розподіл настроїв:
sentiment
unknown     37
negative     7
positive     4
neutral      2
Name: count, dtype: int64

Найчастіші теми:
service               3
atmosphere            1
cleanliness           1
menu explanation      1
portion size          1
pricing               1
vegetarian options    1
menu variety          1
professionalism       1
family                1
Name: count, dtype: int64

Найчастіші пропозиції:
Improve waiter training                   1
Provide clearer menu descriptions         1
increase portion sizes                    1
adjust pricing                            1
add more vegetarian dishes                1
expand the menu options                   1
double-check orders before fulfillment    1
improve wait times for corrections        1
simplify the app interface                1
provide a tutorial for new users          1
Name: count, dtype: int64

Висновок:
За результатами видно, що клієнти найчастіше звертають увагу на якість їжі, сервіс, ціни, доставку та атмосферу. Якщо відгуки негативні, то найчастіше проблема пов'язана з повільним обслуговуванням, холодною їжею або високими цінами. Для покращення ресторану можна зробити швидше обслуговування, додати більше страв у меню, покращити доставку та уважніше перевіряти замовлення.
