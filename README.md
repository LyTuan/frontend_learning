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

5. CSS Function
    - var()
    - rgb()
    - calc()
    - attr()
6. Pseudo classes
    - :root  Tham chiếu đến chính thẻ html của page
    - :hover   Ví dụ: h1:hover, khi hover vào thẻ h1 sẽ sử dụng class này
    - :active  Ví dụ: h1:active, khi click và giữ chuột sẽ sử dụng class này
    - :first-child  Ví dụ: ul:first-child, custom cho phần tử đầu tiên của element ul
    - :last-child Ví dụ: ul:last-child, custom cho phần tử cuối cùng của element ul
7. Đệm, viền, khoảng lề 
    - Padding:
    - Border: 
    - Margin: 
    - Box sizing
        - Là thuộc tính cho phép tự động tính kích thước phần tử. 
        - border-box: tự động chia width cho border, padding và content 
        
8. Background 
    - background-clip: 
        -   Fill background từ vị trí nào. 
        -   content-box: Fill background cho riêng content
        -   padding-box: Fill background cho padding + content 
        -   border-box: Fill background cho border + padding + content 
    - background-url:
        -  Fill background là 1 hình ảnh
        ```
            background-image: linear-gradient(0, rgba(255,255,0, 0.5), rgba(0,0, 255, 0.5)),
            url('https://vcdn-dulich.vnecdn.net/2020/09/04/1-Meo-chup-anh-dep-khi-di-bien-9310-1599219010.jpg');
        ```
