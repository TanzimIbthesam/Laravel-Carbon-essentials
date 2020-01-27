# Laravel-Carbon-essentials
 //For setting the current timezone to Asia Dhaka
    $dt=new Carbon;
    $current=Carbon::now()->timezone('Asia/Dhaka');
    echo $current;
    echo "<br>";
    //To now about yesterday,today and tomorrow dates
    echo $current->today();
    echo "<br>";
    echo $current->yesterday();
    echo "<br>";
    echo $current->tomorrow();
    echo "<br>";
    //To make it readable for humans
    echo $current->diffForHumans();
    echo "<br>";
    $newYear=new Carbon('First day of January');
    echo $newYear->diffForHumans();
    //control date
    echo "<br>";
    echo Carbon::createFromDate(2020,1,27,'Asia/Dhaka');
    echo "<br>";
    //if we want to write about year,days in month and second
 echo $dt->year;
 echo "<br>";
 $date = \Carbon\Carbon::now();
echo $date->format('F'); // July
echo "<br>";
echo $date->subMonth()->format('F'); // Ju
echo "<br>";
echo $dt->toDayDateTimeString();
echo "<br>";
echo $dt->toFormattedDateString();
//
echo "<br>";
//To know hour minutes and second
echo $dt->format('h:i:s A');
//To display previous month
echo Carbon::now()->subMonth()->diffForHumans();
//A month from now
echo "<br>";
echo $dt->toFormattedDateString();
 
