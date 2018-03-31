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


