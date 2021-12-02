### Примеры чек-листов, составленных во время обучения на  «Яндекс.Практикуме»

### Содержание
1. Чек-листы при тестировании функциональности
2. Чек-листы при тестировании API
3. Чек-листы при тестировании мобильного приложения

<h3> Чек-листы при тестировании функциональности </h3> 

#### Окно «Добавление карты» 

> **Требования**  
> 
>
> **Поле «Номер карты»** — 12 символов, только цифры, от 0000 до 9999, проблеы ставятся автоматически, при снятии фокуса, меньше 12 символов кнопка «Привязать» неактивна
> 
> **Поле «Код»** — только цифры, 2 символа, от 00 до 99 включительно, меньше 2 символов, кнопка «Привязать, неактивна.  


<table> 
<tr>
	    <th>№ </th>
	    <th>Описание проверки</th>
        <th>Статус</th>
        <th>Баг-репорт</th>
</tr >
	<tr >
	    <th valign="middle" align="center" rowspan="1"> 1 </th>
	    <td> Проверить, что при открытии окна «Добавление карты» есть поле «Номер карты» и «Код» </td>
        <td valign="middle" align="center" > <span style="color:green"> PASSED </span> </td>
        <td valign="middle" align="center"> </td>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> 2 </th>
	    <td> Проверить, что при открытии окна «Добавление карты» есть неактивная кнопка «Привязать» и активная кнопка «Отмена» </td>
        <td valign="middle" align="center" > <span style="color:green"> PASSED </span> </td>
        <td valign="middle" align="center"> </td>
    </tr>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> 3 </th>
	    <td> Проверить, что при корректном введении данных в поле «Номер» карты» и «Код» отображается активная кнопка «Привязать» </td>
	    <td valign="middle" align="center" > <span style="color:green"> PASSED </span> </td>
        <td valign="middle" align="center"> </td>
    </tr>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> 4 </th>
	    <td> Проверить, что при заполненном поле «Номер карты», но незаполненном поле «Код» кнопка «Привязать» не активна
        <td valign="middle" align="center" > <span style="color:green"> PASSED </span> </td>
        <td valign="middle" align="center"> </td>
    </td>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> 5 </th>
	    <td> Проверить, что при бронировании машины нужно ввести реквизиты хотя бы одной карты и нажать кнопку «Привязать»
        <td valign="middle" align="center" > <span style="color:green"> PASSED </span> </td>
        <td valign="middle" align="center"> </td>
    </td>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> 6 </th>
	    <td> Проверить, что можно добавить 5 банковских карт 
        <td valign="middle" align="center" > <span style="color:green"> PASSED </span> </td>
        <td valign="middle" align="center"> </td>
    </td>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> 7 </th>
	    <td> Проверить, что можно удалить банкоскую карту
        <td valign="middle" align="center" > <span style="color:red"> FAILED </span> </td>
        <td valign="middle" align="center"> </td>
    </td>
    <tr>
	    <th valign="middle" align="center" rowspan="1"> 8 </th>
	    <td> Проверить, что в поле «Номер карты» можно ввести только 12 цифр
        <td valign="middle" align="center" > <span style="color:green"> PASSED </span> </td>
        <td valign="middle" align="center"> </td>
    </td>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> 9 </th>
	    <td> Проверить, что при снятии фокуса с поля «Номер карты» пробелы ставятся автоматически после введения номера
        <td valign="middle" align="center" > <span style="color:red"> FAILED </span> </td>
        <td valign="middle" align="center"> Cсылка на баг-репорт </td>
    </td>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> 10 </th>
	    <td> Проверить, что есть ввести меньше 12 цифр, кнопка «Привязать» остаётся неактивной и появляется сообщение об ошибке «Некорректный номер»
        <td valign="middle" align="center" > <span style="color:green"> PASSED </span> </td>
        <td valign="middle" align="center"> </td>
    </td>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> 11 </th>
	    <td> Проверить, что при введении больше 12 цифр в поле «Номер карты» появляется сообщение об ошибке «Некорректный номер»
        <td valign="middle" align="center" > <span style="color:green"> PASSED </span> </td>
        <td valign="middle" align="center"> </td>
    </td>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> 12 </th>
	    <td> Проверить, что при введении в поле «Номер карты» спецсимволов появляется сообщение об ошибке «Некорректный номер»
        <td valign="middle" align="center" > <span style="color:green"> PASSED </span> </td>
        <td valign="middle" align="center"> Cсылка на баг-репорт </td>
    </td>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> 13 </th>
	    <td> Проверить, что при введении в поле «Номер карты» букв появляется сообщение об ошибке «Некорректный номер»
        <td valign="middle" align="center" > <span style="color:green"> PASSED </span> </td>
        <td valign="middle" align="center"> </td>
    </td>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> 14 </th>
	    <td> Проверить, что при введении в поле «Номер карты» отрицательных цифр появляется сообщение об ошибке «Некорректный номер»
        <td valign="middle" align="center" > <span style="color:green"> PASSED </span> </td>
        <td valign="middle" align="center"> </td>
    </td>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> 15 </th>
	    <td> Проверить, что в поле «Код» можно ввести только 2 цифры
        <td valign="middle" align="center" > <span style="color:red"> FAILED </span> </td>
        <td valign="middle" align="center"> Cсылка на баг-репорт </td>
    </td>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> 16 </th>
	    <td> Проверить, если в поле «Код» ввести букву появится сообщение об ошибке «Некорректный номер»
        <td valign="middle" align="center" > <span style="color:green"> PASSED </span> </td>
        <td valign="middle" align="center"> </td>
    </td>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> 17 </th>
	    <td> Проверить, если в поле «Код» ввести спецсимвол появится сообщение об ошибке «Некорректный номер»
        <td valign="middle" align="center" > <span style="color:red"> FAILED </span> </td>
        <td valign="middle" align="center"> Cсылка на баг-репорт </td>
    </td>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> 18 </th>
	    <td> Проверить, что есть ввести меньше 2 цифр в поле «Код», кнопка «Привязать» остаётся неактивной и появляется сообщение об ошибке «Некорректный номер»
        <td valign="middle" align="center" > <span style="color:green"> PASSED </span> </td>
        <td valign="middle" align="center"> </td>
    </td>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> 19 </th>
	    <td> Проверить, что при введении больше 2 цифр в поле «Код» появляется сообщение об ошибке «Некорректный номер»
        <td valign="middle" align="center" > <span style="color:green"> PASSED </span> </td>
        <td valign="middle" align="center"> </td>
    </td>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> 20 </th>
	    <td> Проверить, что при введении двух нулей (00) в поле «Код» появляется сообщение об ошибке «Некорректный номер»
        <td valign="middle" align="center" > <span style="color:green"> PASSED </span> </td>
        <td valign="middle" align="center"> </td>
    </td>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> 21 </th>
	    <td> Проверить, что при введении в поле «Код» отрицательных цифр появляется сообщение об ошибке «Некорректный номер»
         <td valign="middle" align="center" > <span style="color:green"> PASSED </span> </td>
         <td valign="middle" align="center"> </td>
    </td>

</tr>
</table>

