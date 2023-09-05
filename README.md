# newDataForReference
Новое значение для реквизитов справочника

Например необходимо задать новое значение реквизиту "Наименование" и "НаименованиеПолное" для справочника "Номенклатура"
для этого необходимо в табличный документ добавить строки значений с колонками "Код", "Наименование", "НаименованиеПолное"
в шапке обработки указать наименование справочника = "Номенклатура", а внутреннее соединение ПО = "Код" что позволит
отобрать элементы по коду и установить новые значения соответствующим элементам.

Данная обработка позволит получить метаданные и данные указанного элемента справочника.
Для дополнительных реквизитов (если необходимо установить одинаковое значение всем) как вариант, всем элементам
с указанными кодами можно заменить реквизит комментарий на уникальную строку (например: "a61758ec-045a-11ea-aa6f-c412f5d4ae59")
после чего воспользоваться типовой обработкой "ГрупповоеИзменениеРеквизитов" и отобрав по комментарий установить нужное знч доп. реквизиту.
