    You should have a table with at least three columns and five rows, headers included.

    Cells in the first row should be table headers containing days of the week.
    Cells in the first column should be table headers with a class of time and should contain time values as their text.

    All data cells should have the class of available-#, where # is a number from 0 to 5 that specifies the number of available people at that time.

    In your :root selector, you should define six CSS variables named --color#, where # is a number from 0 to 5, and assign them each a color value. Use these variables to set the background color of the corresponding .available-# elements.


    In your :root selector, you should define CSS variables named --solid-border and --dashed-border. Use these variables to style the bottom borders of your data cells, alternating between solid and dashed borders depending on the row. Give the rows either the class of sharp or half to style them.

    You should have a div element with the id of legend. It should contain a span element with the text Availability and a div element with the id of legend-gradient.
    You should give the #legend-gradient element a linear gradient that transitions between all the colors from --color0 to --color5. Each color value should have two color stops (expressed as percentages) to make the transition between colors a hard line.

<!-- CODIGO HTML QUE FUNCIONA -->

<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Availability Table</title>
  <link rel="stylesheet" href="styles.css">
</head>

<body>
  <main>
    <table>

      <thead>
        <tr>
          <th>&nbsp;</th>
          <th>Monday</th>
          <th>Tuesday</th>
          <th>Wednesday</th>
          <th>Thursday</th>
          <th>Friday</th>
        </tr>
      </thead>

      <tbody>
        <tr class="sharp">
          <th class="time" rowspan="2">9AM</th>
          <td class="available-"></td>
          <td class="available-"></td>
          <td class="available-"></td>
          <td class="available-"></td>
          <td class="available-"></td>
        </tr>

        <tr class="half">
          <td class="available-"></td>
          <td class="available-"></td>
          <td class="available-"></td>
          <td class="available-"></td>
          <td class="available-"></td>
        </tr>

        <tr class="sharp">
          <th class="time" rowspan="2">10AM</th>
          <td class="available-"></td>
          <td class="available-"></td>
          <td class="available-"></td>
          <td class="available-"></td>
          <td class="available-"></td>
        </tr>

        <tr class="half">
          <td class="available-"></td>
          <td class="available-"></td>
          <td class="available-"></td>
          <td class="available-"></td>
          <td class="available-"></td>
        </tr>

        <tr class="sharp">
          <th class="time" rowspan="2">11AM</th>
          <td class="available-"></td>
          <td class="available-"></td>
          <td class="available-"></td>
          <td class="available-"></td>
          <td class="available-"></td>
        </tr>

        <tr class="half">
          <td class="available-"></td>
          <td class="available-"></td>
          <td class="available-"></td>
          <td class="available-"></td>
          <td class="available-"></td>
        </tr>

        <tr class="sharp">
          <th class="time" rowspan="2">12M</th>
          <td class="available-"></td>
          <td class="available-"></td>
          <td class="available-"></td>
          <td class="available-"></td>
          <td class="available-"></td>
        </tr>

        <tr class="half">
          <td class="available-"></td>
          <td class="available-"></td>
          <td class="available-"></td>
          <td class="available-"></td>
          <td class="available-"></td>
        </tr>

        <tr class="sharp">
          <th class="time" rowspan="2">1PM</th>
          <td class="available-"></td>
          <td class="available-"></td>
          <td class="available-"></td>
          <td class="available-"></td>
          <td class="available-"></td>
        </tr>

        <tr class="half">
          <td class="available-"></td>
          <td class="available-"></td>
          <td class="available-"></td>
          <td class="available-"></td>
          <td class="available-"></td>
        </tr>

      </tbody>
    </table>

    <div id="legend">
      <span>Availability</span>
      <div id="legend-gradient">
      </div>
    </div>

  </main>

</body>

</html>

<!-- CODIGO CSS PASA  -->

:root{
--color0: #0000ff;
--color1: #0505be;
--color2: #2c53bd;
--color3: #4242c7;
--color4: #5e5ec0;
--color5: #a1a1e4;
--solid-border: 1px rgb(18, 18, 41);
--dashed-border: 1px white;
}

table{
width: 600px;
height: 200px;
background-color:
color: white;
margin: 0 auto;

}

.available-0{
background-color: var(--color0);
}

.available-1{
background-color: var(--color1);
}
.available-2{
background-color: var(--color2);
}
.available-3{
background-color: var(--color3);
}
.available-4{
background-color: var(--color4);
}
.available-5{
background-color: var(--color5);
}

.sharp td {
height: 40px;
border-bottom: var(--solid-border);
}

.half td{
height: 2px;
border-bottom: var(--dashed-border);
}

#legend{
font-size: 2em;
text-align: center;

}

#legend-gradient{
width: 100px;
height: 20px;
margin: 0px 0 0 450px;
background-image: linear-gradient(
to right,
var(--color0) 0% 15%,
var(--color1) 16% 35%,
var(--color2) 36% 56%,
var(--color3) 57% 77%,
var(--color4) 78% 88%,
var(--color5) 89% 100%
);

}

<!-- codigooooo -->

/\* :root{
--color0: #0000ff;
--color1: #0505be;
--color2: #2c53bd;
--color3: #4242c7;
--color4: #5e5ec0;
--color5: #a1a1e4;
--solid-border: 1px rgb(18, 18, 41);
--dashed-border: 1px white;
}

table{
width: 600px;
height: 200px;
background-color:
color: white;
margin: 0 auto;

}

.available-0{
background-color: var(--color0);
}

.available-1{
background-color: var(--color1);
}
.available-2{
background-color: var(--color2);
}
.available-3{
background-color: var(--color3);
}
.available-4{
background-color: var(--color4);
}
.available-5{
background-color: var(--color5);
}

.sharp td {
height: 40px;
border-bottom: var(--solid-border);
}

.half td{
height: 2px;
border-bottom: var(--dashed-border);
}

#legend{
font-size: 2em;
text-align: center;

}

#legend-gradient{
width: 100px;
height: 20px;
margin: 0px 0 0 450px;
background-image: linear-gradient(
to right,
var(--color0) 0% 15%,
var(--color1) 16% 35%,
var(--color2) 36% 56%,
var(--color3) 57% 77%,
var(--color4) 78% 88%,
var(--color5) 89% 100%
);

} \*/
