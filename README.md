# php-metar
PHP library that parses coded METAR weather reports.

How to use:

Here's an example of METAR data:
KTTN 051853Z 04011KT M1/2SM VCTS SN FZFG BKN003 OVC010 M02/M02 A3006 RMK AO2 TSB40 SLP176 P0002 T10171017=

<?php

include 'Metar.php';

$data = "KTTN 051853Z 04011KT M1/2SM VCTS SN FZFG BKN003 OVC010 M02/M02 A3006 RMK AO2 TSB40 SLP176 P0002 T10171017=";
$metar = new Metar($data);
$result = $metar->parse();

print($result)
