# Chapter03 - 01. CSS 입문

## CSS 기본 형식

```css
div {
    font-size: 20px;
    color: red;
}
```

```
선택자( Selector ) {
    속성( Properties ): 값( Value );
    속성( Properties ): 값( Value );
}
```

> (?) HTML - 속성 : Attribute / CSS - 속성 : Properties

## CSS 선언 방식

#### 인라인 방식

> 태그에 직접 작성 하는 방식

```html
<div style="color: red;">태그</div>
<div style="color: red;">태그</div>
```

#### 내장 방식

> HTML의 <style></style> 안에 포함하는 방식

```html
<head>
    <style>
        div {
            color: red;
        }
    </style>
</head>
<body>
    <div>태그</div>
    <div>태그</div>
</body>
```

#### 외부 CSS 파일 참조 방식

> CSS만 작성 한 별도의 CSS 파일을 HTML 파일에 불러와서 사용 하는 방식

```html
- ooo.html

<head>
    <link rel="stylesheet" href="/css/main.css">
</head>
<body>
    <div>태그</div>
    <div>태그</div>
</body>
```

```css
- /css/main.css

div {
    color: red;
}
```