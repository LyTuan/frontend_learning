# frontend_learning

1. CSS selector

  | Selector | Ví dụ | Mô tả |
  | --- | ----------- | --- |
  |.class|	.intro	| Chọn tất cả các thẻ có class=“intro”|
  |.class1.class2 |	.name1.name2|	Chọn tất cả các thẻ có cả name1 và name2 được đặt trong thuộc tính class của nó|
  |.class1 .class2	|.name1 .name2|	Chọn tất cả các thẻ có class=“name2” là con của một phần tử có class=“name1”|
  |* |	* |	Chọn tất cả các thẻ|
  |element|	h2	|Chọn tất cả các thẻ h2|
  |element.class|	div.box|	Chọn tất cả thẻ div có class=“box”|
  |element, element	|div, h2|	Chọn tất cả thẻ div và h2|
  |element element	|div p	|Chọn tất cả thẻ p trong thẻ div|
  |element > element|	div > p	|Chọn tất cả thẻ p là con trực tiếp của thẻ div|
  |element + element|	div + p|	Chọn thẻ p đứng liền kề sau thẻ div|
  |element ~ element|	div ~ p	|Chọn tất cả thẻ p đứng sau thẻ div|

2. Độ ưu tiên trong CSS
  - Internal và External: Độ ưu tiên phụ thuộc vào việc đặt thẻ link trước thẻ style (Ưu tiên thẻ style hơn vì mới hơn) và ngược lại
  - Inline: 1000 
  - Id: 100
  - Class: 10
  - Tag: 1
  - Equal specific: Cái nào mới hơn (Ở dưới) thì được áp dụng cái đó
