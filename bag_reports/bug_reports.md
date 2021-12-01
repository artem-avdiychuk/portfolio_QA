##### Примеры баг-репортов, составленных во время обучения на  «Яндекс.Практикуме» 

<h4> Тестирование API </h4>

<table> 
<tr>
	    <th>Название поля</th>
	    <th>Содержание</th>
</tr >
	<tr >
	    <th valign="middle" align="center" rowspan="1"> Заголовок </th>
	    <td valign="middle" align="center">В «Яндекс.Прилавке» 200 OK при отправке POST /api/v1/kits/{id}/products при указании отрицательного значения в параметр количества продуктов </td>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> ID </th>
	    <td valign="middle" align="center">BUG-236830 </td>
	</tr>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> Окружение </th>
	    <td valign="middle" align="center"> адрес сервера </td>
	</tr>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> Шаги воспроизведение </th>
	    <td valign="middle" align="center"> отправить POST на /api/v1/kits/{id}/products и указать в количестве продуктов отрицательное значение
    </td>
    <tr >
	    <th valign="middle" align="center" rowspan="1"> Тело </th>
	    <td>
<p align="center">
  <img src="https://github.com/everyrubb/portfolio_QA/blob/main/bag_reports/img.png" width="150" title="hover text">
</p>
</td>
	</tr>
</table>
