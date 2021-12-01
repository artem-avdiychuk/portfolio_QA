### Примеры баг-репортов, составленных во время обучения на  «Яндекс.Практикуме»

#### Содержание
3.1 [Баг-репорт при тестировании функциональности ](https://github.com/everyrubb/portfolio_QA/tree/main/bug_reports#-баг-репорт-при-тестировании-функциональности-)   
3.2 [Баг-репорты при тестировании API](https://github.com/everyrubb/portfolio_QA/tree/main/bug_reports#-баг-репорт-при-тестировании-мобильного-приложения-)  
3.3 [Баг-репорт при тестировании мобильного приложения](https://github.com/everyrubb/portfolio_QA/tree/main/bug_reports#-баг-репорт-при-тестировании-мобильного-приложения-)

<h4> Баг-репорт при тестировании функциональности </h4>

> **Требование:** Возможность удаление банковской карты

<table> 
<tr>
	    <th>Название поля</th>
	    <th>Содержание</th>
</tr >
	<tr >
	    <th valign="middle" align="center" rowspan="1"> Заголовок </th>
	    <td valign="middle" align="center">В «Яндекс.Маршруты. Учебный тренажёр» в окне «Добавление карты» нет возможности удалить банковскую карту
    </td>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> ID </th>
	    <td valign="middle" align="center"> BUG-220477 </td>
	    </tr>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> Описание </th>
	    <td valign="middle" align="center"> В окне «Способ оплаты» нет возможности удалить банковскую карту
     </td>
	    </tr>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> Шаги воспроизведение </th>
	    <td valign="middle" align="center"> 1. Открыть «Яндекс.Маршруты. Учебный тренажёр».
                                        <br>
                                            2. Добавить в поле «Откуда» — Хамовнический Вал, 34
                                        <br>
                                            3. Добавить в поле «Куда» — Зубовский бульвар, 37
                                        <br>
                                            4. Нажать на поле «Добавить банковвскую карту» 
                                        <br>
                                            5. Заполнить поля «Номер карты» и «Код»
                                        <br>
                                            6. Нажать «Привязать»
    </td>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> Ожидаемый результат </th>
	    <td valign="middle" align="center"> Можно удалить банковскую карту
    </td>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> Фактический результат </th>
	    <td valign="middle" align="center"> Нельзя удалить банковскую карту
    </td>
    <tr>
	    <th valign="middle" align="center" rowspan="1"> Приоритет </th>
	    <td valign="middle" align="center"> Средний
    </td>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> Окружение </th>
	    <td valign="middle" align="center"> macOS Catalina версия 10.15.6,
                                        <br>
                                            Яндекс.Браузер 21.8.0.1716 (64-bit) с размером экрана 800x600
    </td>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> Дополнительные материалы </th>
	    <td valign="middle" align="center"> приложить скриншот
    </td>
</tr>
</table>

<h4> Баг-репорт при тестировании API </h4>

> **Требование:** При вводе отрицательных значений возврат 400 Bad request

<table> 
<tr>
	    <th>Название поля</th>
	    <th>Содержание</th>
</tr >
	<tr >
	    <th valign="middle" align="center" rowspan="1"> Заголовок </th>
	    <td valign="middle" align="center">В «Яндекс.Прилавке» 200 OK при отправке POST /api/v1/kits/{id}/products при указании отрицательного значения в параметр количества продуктов
        </td>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> ID </th>
	    <td valign="middle" align="center"> BUG-236830 </td>
	    </tr>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> Окружение </th>
	    <td valign="middle" align="center"> Адрес сервера </td>
	    </tr>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> Шаги воспроизведение </th>
	    <td valign="middle" align="center"> Отправить POST на /api/v1/kits/{id}/products и указать в количестве продуктов отрицательное значение
    </td>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> Тело </th>
	    <td> <p align="center"> <img src="https://github.com/everyrubb/portfolio_QA/blob/main/bug_reports/img.png" width="150" title="hover text"></p>
    </td>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> Ожидаемый результат </th>
	    <td valign="middle" align="center"> В ответе ошибка — 400 Bad request и «нельзя добавить в количество товаров отрицательное число»
    </td>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> Фактический результат </th>
	    <td valign="middle" align="center"> 200 ОК, в ответ уменьшается количество ранее добавленных продуктов
    </td>
    <tr>
	    <th valign="middle" align="center" rowspan="1"> Приоритет </th>
	    <td valign="middle" align="center"> Критичный
    </td>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> Дополнительные материалы </th>
	    <td valign="middle" align="center"> приложить логи, ответ от сервера
    </td>


</tr>
</table>

<h4> Баг-репорт при тестировании мобильного приложения </h4>

> **Требование:** При интернет-соединении приложение не работает

<table> 
<tr>
	    <th>Название поля</th>
	    <th>Содержание</th>
</tr >
	<tr >
	    <th valign="middle" align="center" rowspan="1"> Заголовок </th>
	    <td valign="middle" align="center"> В «Яндекс.Метро» при отсутствии интернет-соединения приложение продолжает корректно работать
    </td>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> ID </th>
	    <td valign="middle" align="center"> BUG-236730 </td>
	    </tr>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> Описание </th>
	    <td valign="middle" align="center"> В «Яндекс.Метро» при отсутствии интернет-соединения приложение продолжает корректно работать
     </td>
	    </tr>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> Шаги воспроизведение </th>
	    <td valign="middle" align="center"> 1. Отключить в настройках телефона Wi-Fi и мобильный интернет.
                                        <br>
                                            2. Открыть «Яндекс.Метро»
                                        <br>
                                            3. Добавить в поле «Откуда» — «Сокол»
                                        <br>
                                            4. Добавить в поле «Куда» — «Охотный ряд»
                                        <br>
                                            5. Отключить интернет-соединение
    </td>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> Ожидаемый результат </th>
	    <td valign="middle" align="center"> Появляется уведомление об отсутствии интернета
    </td>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> Фактический результат </th>
	    <td valign="middle" align="center"> Приложение продолжает корректно работать
    </td>
    <tr>
	    <th valign="middle" align="center" rowspan="1"> Приоритет </th>
	    <td valign="middle" align="center"> Средний
    </td>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> Окружение </th>
	    <td valign="middle" align="center"> Хiaomi Mi 4W, Android 6.0.1
    </td>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> Дополнительные материалы </th>
	    <td valign="middle" align="center"> приложить скриншоткаст или скриншот 
    </td>
</tr>
</table>