# Описание интерфейса IPay
Интерфейс предназначен для работы с методами класса Pay

## Реализация интерфейса
* + Add (Pay: [Pay](Pay.md)): Int — функция, добавляющая платёж в базу данных.
* + Delete(ID : Int) : Bool Функция удаляющая платёж
* + FindByID(ID : int) : [Pay](Pay.md)  функция, осуществляющая поиск платежа в базе данных по ID и возвращающая найденный, если такой есть.
* + GetAllPay(sorting : String, filtering : String, sortingA : boolean, count : int, page : int) : [Manager](Manager.md) функция получающая список платежей
Параметры:
	* sortinig: string — отвечает, по какому полю будет сортироваться список;
	* sortingA: bool — отвечает, по возрастанию или убыванию будут сортироваться элементы;
	* filtering: string — отвечает за фильтрацию;
	* count: int — отвечает, сколько элементов необходимо показать;
	* page: int — отвечает, с какой страницы начинать поиск элементов.
* + Save(Pay : [Pay](Pay.md)) : Bool функция, редактирующая данные о платеже.