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
    - Important: Khi khai báo key này, nó sẽ ưu tiên hơn cả inline
    - Inheritant: Kế thừa từ thuộc tính cha

3. Đặt tên cho biến CSS

```
#Khai báo biến global
:root {
  --text-color: red;
}
h1 {
  #Khai báo biến local
  --my-font-size: 12px;
  color: var(--text-color);
  font-size: var(--my-font-size);
}
```

4. Đơn vị trong CSS
    - px
    - %: Phụ thuộc vào thẻ chứa nó
    - rem: Phụ thuộc vào thẻ html
    - em: Phụ thuộc vào thẻ gần nhất chứa nó
    - vw (viewport-width): Tỉ lệ phần trăm với chiều ngang trình duyêt (Khác với đơn vị % là đơn vị % phụ thuộc thẻ chứa nó)
    - vh (viewport-hight): Tỉ lệ phần trăm với chiều dài trình duyêt
