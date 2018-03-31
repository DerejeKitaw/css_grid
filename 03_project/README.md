### Add seven dive tags in the index
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>CSS Grid</title>
    <link rel="stylesheet" type="text/css" href="./style/style.css">
</head>
<body>
    <div class="wrapper">
<div class="box box1">Box 1</div>
<div class="box box2">Box 2</div>
<div class="box box3">Box 3</div>
<div class="box box4">Box 4</div>
    </div>
</body>
</html>
```
```css
.wrapper{
    display: grid;
}

.wrapper >div{
    background: #eee;
    padding: 1em;
}
.wrapper >div:nth-child(odd){
    background: #ddd;
}
```
![css_grid](./DOC/css_grid_project3_1.png)
### Create 3 columns with 1fr 2fr and 1fr
```css
.wrapper{
    display: grid;
    grid-template-columns: 1fr 2fr 1fr;
}
```
![css_grid](./DOC/css_grid_project3_2.png)
### Add auto rows
```css
.wrapper{
    display: grid;
    grid-template-columns: 1fr 2fr 1fr;
    grid-auto-rows: minmax(100px, auto);
}
```
![css_grid](./DOC/css_grid_project3_3.png)
### Add grid gap
```css
.wrapper{
    display: grid;
    grid-template-columns: 1fr 2fr 1fr;
    grid-auto-rows: minmax(100px, auto);
    grid-gap: 1em;
}
```
![css_grid](./DOC/css_grid_project3_4.png)
### Align all item to their start point
```css
.wrapper{
    display: grid;
    grid-template-columns: 1fr 2fr 1fr;
    grid-auto-rows: minmax(100px, auto);
    grid-gap: 1em;
    justify-items: start;
}
```
![css_grid](./DOC/css_grid_project3_5.png)
### Justify all item to their start point
```css
.wrapper{
    display: grid;
    grid-template-columns: 1fr 2fr 1fr;
    grid-auto-rows: minmax(100px, auto);
    grid-gap: 1em;
    justify-items: center;
}
```
![css_grid](./DOC/css_grid_project3_6.png)
> compare it with out justify-item

![css_grid](./DOC/css_grid_project3_2.png)
![css_grid](./DOC/css_grid_project3_7.png)
![css_grid](./DOC/css_grid_project3_8.png)
### Align all item to their start point
```css
.wrapper{
    display: grid;
    grid-template-columns: 1fr 2fr 1fr;
    grid-auto-rows: minmax(100px, auto);
    grid-gap: 1em;
    justify-items: stretch;
    align-items: stretch;
}
```
![css_grid](./DOC/css_grid_project3_9.png)
### Align individual item to their start point using `align-self`
```css
.box1{
    align-self: center;
}
.box2{
    align-self: start;
}
.box4{
    align-self: end;
}
```
![css_grid](./DOC/css_grid_project3_10.png)

###

![css_grid](./DOC/css_grid_project3_11.png)
![css_grid](./DOC/css_grid_project3_12.png)
![css_grid](./DOC/css_grid_project3_13.png)