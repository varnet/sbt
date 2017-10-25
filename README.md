# sbt
Simplified Benchmark Test


<?php

/* Simplified Benchmark Test by VR:2017 */

$start = Timer();

for ($i = 0; $i < 10000; $i++) {
    for ($j = 0; $j < 10000; $j++) {
        // any action
    }
}

$stop = Timer();
$trun = round($stop-$start,3);

echo $trun."s\n";

function Timer() {
    list($usec, $sec) = explode(" ", microtime());
    return ((float)$usec + (float)$sec);
}

?>
