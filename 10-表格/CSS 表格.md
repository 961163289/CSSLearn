## CSS 表格

使用 CSS 可以使 HTML 表格更美观

| Company                      | Contact            | Country |
| :--------------------------- | :----------------- | :------ |
| Alfreds Futterkiste          | Maria Anders       | Germany |
| Berglunds snabbköp           | Christina Berglund | Sweden  |
| Centro comercial Moctezuma   | Francisco Chang    | Mexico  |
| Ernst Handel                 | Roland Mendel      | Austria |
| Island Trading               | Helen Bennett      | UK      |
| Königlich Essen              | Philip Cramer      | Germany |
| Laughing Bacchus Winecellars | Yoshi Tannamuri    | Canada  |
| Magazzini Alimentari Riuniti | Giovanni Rovelli   | Italy   |
| North/South                  | Simon Crowther     | UK      |
| Paris spécialités            | Marie Bertrand     | France  |
| The Big Cheese               | Liz Nixon          | USA     |
| Vaffeljernet                 | Palle Ibsen        | Denmark |

### 表格边框

指定CSS表格边框，使用border属性。

下面的例子指定了一个表格的 TH 和 TD 元素的黑色边框：

```css
table, th, td
{
    border: 1px solid black;
}
```

请注意，在上面的例子中的表格有双边框。这是因为表和TH/TD元素有独立的边界。

为了显示一个表的单个边框，使用 border-collapse 属性。

### 折叠边框

border-collapse 属性设置表格的边框是否被折叠成一个单一的边框或隔开：

```css
table
{
    border-collapse:collapse;
}
table,th, td
{
    border: 1px solid black;
}
```

### 表格高度和宽度

Width 和 Height 属性定义表格的宽度和高度。

下面的例子是设置100%的宽度，50像素的TH元素的高度的表格：

```css
table 
{
    width:100%;
}
th
{
    height:50px;
}
```

