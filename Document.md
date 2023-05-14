* Sass Concept
1. Biến trong Sass
- Đặt tên biến:
    $mainTextColor:orange
    Tách tất cả các biến vào một file

2. Nested
nav {
    ul{
        margin:0px;
        padding: 0px;
        list-style-type: none;
        li{
            display: inline-block;
            a{
                display: block;
                text-decoration: none;
                color:$textColor;
                font-size: $normalSize;
                padding: 15px;
                background: $linkBgColor;

                &:hover{
                    background-color: $bgHover;
                    color: $textHover;
                }
            }
        }
    }
}

3. Mixin
- Cú pháp khai báo
    @mixin mixinName{
        css attribute1
        css attribute2
    }
- Sử dụng
    @include mixinName;

4. Extend
5. If else
6. Loop(for, foreach)
7. function
- Khai báo
    @function nameFunction($param, $param2, ...){
        @return value
    }
