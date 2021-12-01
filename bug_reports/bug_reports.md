##### Примеры баг-репортов, составленных во время обучения на  «Яндекс.Практикуме» 

<h4> Тестирование API </h4>

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
    <tr >
	    <th valign="middle" align="center" rowspan="1"> Дополнительные материалы </th>
	    <td valign="middle" align="center"> приложить логи, ответ от сервера
    </td>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> Приоритет </th>
	    <td valign="middle" align="center"> Критичный
    </td>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> Дополнительные материалы </th>
	    <td valign="middle" align="center"> приложить логи, ответ от сервера
    </td>


</tr>
</table>
