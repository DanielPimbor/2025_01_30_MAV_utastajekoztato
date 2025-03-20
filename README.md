## MÁV utastájékoztató

Ez a projekt egy egyszerű módot kínál arra, hogy táblázatos formában értesüljünk a vonatok indulási és érkezési időpontjairól.

Az oldal jelenleg fiktív adatokat tartalmaz (a MÁV API integrációja még fejlesztés alatt áll).

## Extra funkciók 🔥

- a valós, real time idő kijelzése (Credit: Varga Atilla, és az internet)

A projekt elérhető ezen a linken: [🔗 MÁV utastájékoztató](https://danielpimbor.github.io/2025_01_30_MAV_utastajekoztato/)

## 🏢 Alap HTML szerkezet
    ```html
    <!DOCTYPE html>
    <html lang="hu">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>MÁV utastájékoztató</title>
        <link rel="stylesheet" href="indulo_vonatok.css">
    </head>
    <body>
        <table id="indulo">
            <thead>
                <tr>
                    <th id="ido">08:43:10</th>
                    <th>Abfahrt</th>
                    <th colspan="2">Induló vontatok</th>
                    <th>Departures</th>
                    <th><img src="mav.png" alt="MavKep"></th>
                </tr>
                <tr>
                    <th>Tervezett Indulás</th>
                    <th>Indulás</th>
                    <th>Vonat</th>
                    <th>Honnan</th>
                    <th>Hova</th>
                    <th>Vágány</th>
                </tr>
    ```
## 🎵 CSS Stílusok
    ```css
    table, th, td {
    border: 1px solid;
    border-collapse: collapse;
  }

table{
    width: 80%; /* weboldal szélessége */
    background-color: rgb(10, 47, 116); /* háttérszín */
    color: white; /* betűszín */
    font-family: 'Courier New'; /* betűtípus */
    font-size: 25px;
}
th {
    background-color: rgb(30, 63, 133);
}
#keses{
    background-color: red;
}
    ```