HTML:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Page Layout</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="c">
        <div class="box red">
            <div class="icon">&#9997;</div>
        </div>
        <div class="box skin">23/EE/104</div>
        <div class="box purple">
            <div class="icon">&#128065;</div>
        </div>
        <div class="box black center">Himanshu Bhadu</div>
        <div class="box green">Works</div>
        <div class="box bottom">Fear & Failures</div>
    </div>
</body>
</html>

CSS:
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
body {
    font-family: 'Arial';
    font-style: italic;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    background-color: black;
}
.c{
    display: grid;
    height: 80vh;
    width: 80vw;
    gap: 10px;
    grid-template-rows: 1fr 1fr 1fr;
    grid-template-columns: 1fr 1fr 1fr;
}
.box {
    display: flex;
    color: #ffffff;
    border-radius: 15px;
    justify-content: center;
    align-items: center;
    font-size: 2em;
    font-weight: bold;
}
.red {
    background-color: #E74C3C;
    grid-column: 1 / 2;
    grid-row: 1 / 3;
}
.purple {
    background-color: #9B59B6;
    grid-row: 1/3;
}
.skin {
    background-color: #FAD7A0;
    color: #000000;
    font-family: Apple Chancery, cursive;
    text-align: center;
}
.bottom {
    background-color: #FAD7A0;
    color: #000000;
    font-family: OCR A Std, monospace;
    text-align: center;
}
.green {
    background-color: #0aad4e;
    font-family: Apple Chancery, cursive;
    color: #000;
    grid-column: 1 / 3;
}
.black {
    background-color: #000;
    font-size: 2em;
    grid-column: 2 / 3;
    grid-row: 2 / 3;
    font-family: 'Cursive', sans-serif;
}
.icon {
    font-size: 2em;
}
