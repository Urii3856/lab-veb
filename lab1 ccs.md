body {
    font-family: "Times New Roman", Times, serif;
    background-color: black;
    color: yellow;
    margin: 20px;
}

table.layout {
    width: 100%;
    border-collapse: collapse;
    border: 1px solid yellow;
    margin-bottom: 25px;
}

table.layout td {
    border: 1px solid yellow;
    padding: 10px;
    vertical-align: top;
}

.fixed-cell {
    width: 140px;
}

.comp-img {
    border: 0;
    float: left;
    margin: 10px 15px 25px 30px;
    
    /* Задаємо точні розміри картинки, щоб координати картографії збігалися */
    width: 600px;
    height: auto;
}

.clear {
    clear: both;
}

a {
    color: #00ffff;
}

/* Блок підказки над зображенням */
.status-box {
    background-color: #111;
    color: #888;
    border: 1px solid yellow;
    padding: 10px 15px;
    font-size: 18px;
    margin-bottom: 15px;
    width: fit-content;
    border-radius: 5px;
    transition: all 0.2s ease;
}

/* Коли курсор наведений на елемент */
.status-box.active {
    background-color: #002b36;
    color: #00ffff;
    border-color: #00ffff;
    font-weight: bold;
}
