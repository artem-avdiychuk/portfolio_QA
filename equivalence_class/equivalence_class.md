## Классы эквивалетности  

> На веб-сайте заказа такси есть поля «Времени начала поездки, «Откуда» и «Куда» 
>
**Задание:**
> Необходимо выделить классы эквалентности и граничные значения для полей ввода.   
>
****
#### Классы эквивалентности для поля «Время начала поездки»

> **Требования:** формат 24 часа, целые числа от 0 до 23, ноль перед однозначным числом
>
**Макет**  



<table>
	<tr>
	    <th>Группы проверок</th>
	    <th>Название класса</th>
	    <th>Границы</th>  
        <th>Тестовые данные внутри класса (содержимое поля) </th>  
        <th>Тестовые заднные на границах</th>
	</tr >
	<tr >
	    <th valign="middle" align="center" rowspan="13"> Время начала поездки. Часы</th>
	    <td valign="middle" align="center"> 00-09</td>
	    <td valign="middle" align="center"> 00,09</td>
        <td valign="middle" align="center"> 05</td>
        <td valign="middle" align="center"> 00, 09, 01, 08, -01, 10</td>
	</tr>
	<tr>
	    <td valign="middle" align="center"> 10-23</td>
	    <td valign="middle" align="center"> 10,23</td>
        <td valign="middle" align="center"> 15</td>
        <td valign="middle" align="center"> 10, 23, 09, 22, 9, 24</td>
	</tr>
	<tr>
	    <td valign="middle" align="center"> >=24 </td>
	    <td valign="middle" align="center"> 24</td>
        <td valign="middle" align="center"> 30</td>
        <td valign="middle" align="center"> 24, 23 ,25</td>
	</tr>
	<tr>
	    <td valign="middle" align="center"> 2 символа</td>
	    <td valign="middle" align="center"> Набор </td>
        <td valign="middle" align="center"> 15 </td>
        <td> </td>
	</tr>
	<tr>
        <td valign="middle" align="center"> Меньше 2 символов </td>
	    <td valign="middle" align="center">  Набор </td>
        <td valign="middle" align="center"> 1 </td>
        <td> </td>
	</tr>
	<tr>
	    <td valign="middle" align="center"> Больше 2 символов </td>
	    <td valign="middle" align="center">  Набор </td>
        <td valign="middle" align="center"> 111 </td>
        <td> </td>
	</tr>
	<tr>
	    <td valign="middle" align="center"> Отрицательные числа</td>
	    <td valign="middle" align="center">  Набор </td>
        <td valign="middle" align="center">  -01 </td>
        <td> </td>
	</tr>
	<tr>
	    <td valign="middle" align="center"> Дробные числа</td>
	    <td valign="middle" align="center">  Набор </td>
        <td valign="middle" align="center">  2,4 </td>
        <td> </td>
	</tr>
	<tr>
	    <td valign="middle" align="center"> Буква</td>
	    <td valign="middle" align="center">  Набор </td>
        <td valign="middle" align="center">  ВВ </td>
        <td> </td>
	</tr>
	<tr>
        <td valign="middle" align="center"> Без нуля в начале при однозначных числах</td>
        <td valign="middle" align="center">  Набор </td>
        <td valign="middle" align="center">  1 </td>
        <td> </td>
	</tr>
	<tr>
	    <td valign="middle" align="center"> Поле заполнено</td>
	    <td valign="middle" align="center">  Набор </td>
        <td valign="middle" align="center">  01 </td>
        <td> </td>
	</tr>
	<tr>
	    <td valign="middle" align="center"> Поле пустое</td>
	    <td valign="middle" align="center">  Набор </td>
        <td valign="middle" align="center">   </td>
        <td> </td>
	</tr>
	<tr>
	    <td valign="middle" align="center"> Спецсимволы</td>
	    <td valign="middle" align="center"> Набор </td>
        <td valign="middle" align="center">  3# </td>
        <td> </td>
	</tr>
</table>

<table>
	<tr>
	    <th>Группы проверок</th>
	    <th>Название класса</th>
	    <th>Границы</th>  
        <th>Тестовые данные внутри класса (содержимое поля) </th>  
        <th>Тестовые заднные на границах</th>
	</tr >
	<tr >
	    <th valign="middle" align="center" rowspan="13"> Время начала поездки. Минуты</th>
        <td valign="middle" align="center"> 00-09</td>
	    <td valign="middle" align="center"> 00,09</td>
        <td valign="middle" align="center"> 05</td>
        <td valign="middle" align="center"> 00, 09, 01, 08, -01, 10</td>
	</tr>
	<tr>
	    <td valign="middle" align="center"> 10-59</td>
	    <td valign="middle" align="center"> 10,59</td>
        <td valign="middle" align="center"> 30</td>
        <td valign="middle" align="center"> 10, 59, 11, 58, 09, 60</td>
	</tr>
	<tr>
	    <td valign="middle" align="center"> >=60 </td>
	    <td valign="middle" align="center"> 60</td>
        <td valign="middle" align="center"> 75</td>
        <td valign="middle" align="center"> 60, 59, 61</td>
	</tr>
	<tr>
	    <td valign="middle" align="center"> 2 символа</td>
	    <td valign="middle" align="center"> Набор </td>
        <td valign="middle" align="center"> 15 </td>
        <td> </td>
	</tr>
	<tr>
        <td valign="middle" align="center"> Меньше 2 символов </td>
	    <td valign="middle" align="center">  Набор </td>
        <td valign="middle" align="center"> 1 </td>
        <td> </td>
	</tr>
	<tr>
	    <td valign="middle" align="center"> Больше 2 символов </td>
	    <td valign="middle" align="center">  Набор </td>
        <td valign="middle" align="center"> 111 </td>
        <td> </td>
	</tr>
	<tr>
	    <td valign="middle" align="center"> Отрицательные числа</td>
	    <td valign="middle" align="center">  Набор </td>
        <td valign="middle" align="center">  -01 </td>
        <td> </td>
	</tr>
	<tr>
	    <td valign="middle" align="center"> Дробные числа</td>
	    <td valign="middle" align="center">  Набор </td>
        <td valign="middle" align="center">  2,4 </td>
        <td> </td>
	</tr>
	<tr>
	    <td valign="middle" align="center"> Буква</td>
	    <td valign="middle" align="center">  Набор </td>
        <td valign="middle" align="center">  ВВ </td>
        <td> </td>
	</tr>
	<tr>
        <td valign="middle" align="center"> Без нуля в начале при однозначных числах</td>
        <td valign="middle" align="center">  Набор </td>
        <td valign="middle" align="center">  1 </td>
        <td> </td>
	</tr>
	<tr>
	    <td valign="middle" align="center"> Поле заполнено</td>
	    <td valign="middle" align="center">  Набор </td>
        <td valign="middle" align="center">  01 </td>
        <td> </td>
	</tr>
	<tr>
	    <td valign="middle" align="center"> Поле пустое</td>
	    <td valign="middle" align="center">  Набор </td>
        <td valign="middle" align="center">   </td>
        <td> </td>
	</tr>
	<tr>
	    <td valign="middle" align="center"> Спецсимволы</td>
	    <td valign="middle" align="center"> Набор </td>
        <td valign="middle" align="center">  3# </td>
        <td> </td>
    </tr>
</table>

****
#### Классы эквивалентности для поля «Откуда» и «Куда»
> **Требования:** не более 50 сиволов, русские буквы, цифры, пробел, тире, точка, запятая
>
<table>
	<tr>
	    <th>Группы проверок</th>
	    <th>Название класса</th>
	    <th>Границы</th>  
        <th>Тестовые данные внутри класса (содержимое поля) </th>  
        <th>Тестовые заднные на границах</th>
	</tr >
	<tr >
	    <th valign="middle" align="center" rowspan="17">Откуда</th>
        <td valign="middle" align="center"> 1-50</td>
	    <td valign="middle" align="center"> 1, 50</td>
        <td valign="middle" align="center"> <strong> 13 символов </strong> — Комсомольский</td>
        <td valign="middle" align="center"> <strong> 1 символ </strong> — Я,
                                                <br>
                                            <strong> 50 символов </strong>  — проезд Старый Престарый Петровско-Разумовский Петр,
                                                <br>
                                            <strong> 2 символов </strong> — Ян, 
                                                 <br>
                                            <strong> 49 символов </strong> —проезд Старый Престарый Петровско-Разумовский Яша,
                                                <br>
                                            <strong> 0 символов </strong> — пустое поле, 
                                                <br>
                                            <strong> 51 символ </strong> — проезд Старый Престарый Петровско-Разумовский Петра <br>
</td>
	</tr>
	<tr>
	    <td valign="middle" align="center"> 0 </td>
	    <td valign="middle" align="center"> 0 </td>
        <td valign="middle" align="center"> <strong> 0 символов </strong> — пустое поле </td>
        <td valign="middle" align="center"> <strong> 0 символов </strong> — пустое поле
                                                <br>
                                            <strong> 1 символ </strong> — 1 </td>
	</tr>
	<tr>
	    <td valign="middle" align="center"> >=51 </td>
	    <td valign="middle" align="center"> 51 </td>
        <td valign="middle" align="center"> <strong> 52 символов </strong> — проезд Старый Престарый Петровско-Разумовский Петров  </td>
        <td valign="middle" align="center"> <strong> 50 символов </strong> — проезд Старый Престарый Петровско-Разумовский Петр,
                                                <br>
                                            <strong>  50 символов </strong>  — проезд Старый Престарый Петровско-Разумовский Петр
                                                <br>
                                            <strong>  52 символов </strong> — проезд Старый Престарый Петровско-Разумовский Петров" </td>
	</tr>
	<tr>
	    <td valign="middle" align="center"> Строка, состоящая из русских букв </td>
	    <td valign="middle" align="center"> Набор </td>
        <td valign="middle" align="center"> Комсомольский </td>
        <td> </td>
	</tr>
	<tr>
        <td valign="middle" align="center"> Строка, состоящая символов из других языков </td>
	    <td valign="middle" align="center">  Набор </td>
        <td valign="middle" align="center"> Komsomolskiy </td>
        <td> </td>
	</tr>
	<tr>
	    <td valign="middle" align="center"> Строка, содержащая цифры </td>
	    <td valign="middle" align="center">  Набор </td>
        <td valign="middle" align="center"> Комсомольский18 </td>
        <td> </td>
	</tr>
	<tr>
	    <td valign="middle" align="center"> Строка, содержащая тире </td>
	    <td valign="middle" align="center">  Набор </td>
        <td valign="middle" align="center"> Комсомольский—18 </td>
        <td> </td>
	</tr>
	<tr>
	    <td valign="middle" align="center"> Строка, содержащая точку </td>
	    <td valign="middle" align="center">  Набор </td>
        <td valign="middle" align="center"> Комсомольский. </td>
        <td> </td>
	</tr>
	<tr>
	    <td valign="middle" align="center"> Строка, содержащая запятую </td>
	    <td valign="middle" align="center">  Набор </td>
        <td valign="middle" align="center">  Комсомольский, </td>
        <td> </td>
	</tr>
	<tr>
        <td valign="middle" align="center"> Строка, содержащая пробел в начале текста </td>
        <td valign="middle" align="center">  Набор </td>
        <td valign="middle" align="center"> _Комсомольский </td>
        <td> </td>
	</tr>
	<tr>
	    <td valign="middle" align="center"> Строка, содержащая пробел после текста</td>
	    <td valign="middle" align="center">  Набор </td>
        <td valign="middle" align="center">  Комсомольский_ </td>
        <td> </td>
	</tr>
	<tr>
	    <td valign="middle" align="center"> Строка, содержащая пробел в середине текста </td>
	    <td valign="middle" align="center">  Набор </td>
        <td valign="middle" align="center"> Комсомольский_проспект </td>
        <td> </td>
	</tr>
	<tr>
	    <td valign="middle" align="center"> Строка, содержащая спецсимвол</td>
	    <td valign="middle" align="center"> Набор </td>
        <td valign="middle" align="center">  Комсомольский$ </td>
        <td> </td>
    </tr>
	<tr>
	    <td valign="middle" align="center"> Строка, содержащая букву Ё</td>
	    <td valign="middle" align="center"> Набор </td>
        <td valign="middle" align="center">  Усачёва </td>
        <td> </td>
    </tr>
	<tr>
	    <td valign="middle" align="center"> Строка, содержащая адрес не из списка доступных адресов</td>
	    <td valign="middle" align="center"> Набор </td>
        <td valign="middle" align="center">  проезд Старый Престарый Петровско-Разумовский Петров </td>
        <td> </td>
    </tr>
	<tr>
	    <td valign="middle" align="center"> Поле заполнено</td>
	    <td valign="middle" align="center"> Набор </td>
        <td valign="middle" align="center">  Комсомольский </td>
        <td> </td>
    </tr>
	<tr>
	    <td valign="middle" align="center"> Поле пустое</td>
	    <td valign="middle" align="center"> Набор </td>
        <td> </td>
        <td> </td>
    </tr>
</table>

<table>
	<tr>
	    <th>Группы проверок</th>
	    <th>Название класса</th>
	    <th>Границы</th>  
        <th>Тестовые данные внутри класса (содержимое поля) </th>  
        <th>Тестовые заднные на границах</th>
	</tr >
	<tr >
	    <th valign="middle" align="center" rowspan="17">Куда</th>
        <td valign="middle" align="center"> 1-50</td>
	    <td valign="middle" align="center"> 1, 50</td>
        <td valign="middle" align="center"> <strong> 13 символов </strong> — Комсомольский</td>
        <td valign="middle" align="center"> <strong> 1 символ </strong> — Я,
                                                <br>
                                            <strong> 50 символов </strong>  — проезд Старый Престарый Петровско-Разумовский Петр,
                                                <br>
                                            <strong> 2 символов </strong> — Ян, 
                                                 <br>
                                            <strong> 49 символов </strong> —проезд Старый Престарый Петровско-Разумовский Яша,
                                                <br>
                                            <strong> 0 символов </strong> — пустое поле, 
                                                <br>
                                            <strong> 51 символ </strong> — проезд Старый Престарый Петровско-Разумовский Петра <br>
</td>
	</tr>
	<tr>
	    <td valign="middle" align="center"> 0 </td>
	    <td valign="middle" align="center"> 0 </td>
        <td valign="middle" align="center"> <strong> 0 символов </strong> — пустое поле </td>
        <td valign="middle" align="center"> <strong> 0 символов </strong> — пустое поле
                                                <br>
                                            <strong> 1 символ </strong> — 1 </td>
	</tr>
	<tr>
	    <td valign="middle" align="center"> >=51 </td>
	    <td valign="middle" align="center"> 51 </td>
        <td valign="middle" align="center"> <strong> 52 символов </strong> — проезд Старый Престарый Петровско-Разумовский Петров  </td>
        <td valign="middle" align="center"> <strong> 50 символов </strong> — проезд Старый Престарый Петровско-Разумовский Петр,
                                                <br>
                                            <strong>  50 символов </strong>  — проезд Старый Престарый Петровско-Разумовский Петр
                                                <br>
                                            <strong>  52 символов </strong> — проезд Старый Престарый Петровско-Разумовский Петров" </td>
	</tr>
	<tr>
	    <td valign="middle" align="center"> Строка, состоящая из русских букв </td>
	    <td valign="middle" align="center"> Набор </td>
        <td valign="middle" align="center"> Комсомольский </td>
        <td> </td>
	</tr>
	<tr>
        <td valign="middle" align="center"> Строка, состоящая символов из других языков </td>
	    <td valign="middle" align="center">  Набор </td>
        <td valign="middle" align="center"> Komsomolskiy </td>
        <td> </td>
	</tr>
	<tr>
	    <td valign="middle" align="center"> Строка, содержащая цифры </td>
	    <td valign="middle" align="center">  Набор </td>
        <td valign="middle" align="center"> Комсомольский18 </td>
        <td> </td>
	</tr>
	<tr>
	    <td valign="middle" align="center"> Строка, содержащая тире </td>
	    <td valign="middle" align="center">  Набор </td>
        <td valign="middle" align="center"> Комсомольский—18 </td>
        <td> </td>
	</tr>
	<tr>
	    <td valign="middle" align="center"> Строка, содержащая точку </td>
	    <td valign="middle" align="center">  Набор </td>
        <td valign="middle" align="center"> Комсомольский. </td>
        <td> </td>
	</tr>
	<tr>
	    <td valign="middle" align="center"> Строка, содержащая запятую </td>
	    <td valign="middle" align="center">  Набор </td>
        <td valign="middle" align="center">  Комсомольский, </td>
        <td> </td>
	</tr>
	<tr>
        <td valign="middle" align="center"> Строка, содержащая пробел в начале текста </td>
        <td valign="middle" align="center">  Набор </td>
        <td valign="middle" align="center"> _Комсомольский </td>
        <td> </td>
	</tr>
	<tr>
	    <td valign="middle" align="center"> Строка, содержащая пробел после текста</td>
	    <td valign="middle" align="center">  Набор </td>
        <td valign="middle" align="center">  Комсомольский_ </td>
        <td> </td>
	</tr>
	<tr>
	    <td valign="middle" align="center"> Строка, содержащая пробел в середине текста </td>
	    <td valign="middle" align="center">  Набор </td>
        <td valign="middle" align="center"> Комсомольский_проспект </td>
        <td> </td>
	</tr>
	<tr>
	    <td valign="middle" align="center"> Строка, содержащая спецсимвол</td>
	    <td valign="middle" align="center"> Набор </td>
        <td valign="middle" align="center">  Комсомольский$ </td>
        <td> </td>
    </tr>
	<tr>
	    <td valign="middle" align="center"> Строка, содержащая букву Ё</td>
	    <td valign="middle" align="center"> Набор </td>
        <td valign="middle" align="center">  Усачёва </td>
        <td> </td>
    </tr>
	<tr>
	    <td valign="middle" align="center"> Строка, содержащая адрес не из списка доступных адресов</td>
	    <td valign="middle" align="center"> Набор </td>
        <td valign="middle" align="center">  проезд Старый Престарый Петровско-Разумовский Петров </td>
        <td> </td>
    </tr>
	<tr>
	    <td valign="middle" align="center"> Поле заполнено</td>
	    <td valign="middle" align="center"> Набор </td>
        <td valign="middle" align="center">  Комсомольский </td>
        <td> </td>
    </tr>
	<tr>
	    <td valign="middle" align="center"> Поле пустое</td>
	    <td valign="middle" align="center"> Набор </td>
        <td> </td>
        <td> </td>
    </tr>
</table>