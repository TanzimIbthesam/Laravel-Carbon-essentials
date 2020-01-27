# Laravel-Carbon-essentials
Carbon Notes 

For specifying a time zone if you want current time zone like you want exact time of Dhaka 
$current=Carbon::now()->timezone('Asia/Dhaka');
    echo $current;
To now about yesterday,today and tomorrow dates
    echo $current->today();
    echo "<br>";
    echo $current->yesterday();
    echo "<br>";
    echo $current->tomorrow();
To find out in readableformat what time is it 
