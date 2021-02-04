# convert number Bangla to English

~~~php
<?php
 public function bn2enNumber ($number){
    $search_array= array("১", "২", "৩", "৪", "৫", "৬", "৭", "৮", "৯", "০");
    $replace_array= array("1", "2", "3", "4", "5", "6", "7", "8", "9", "0");
    $en_number = str_replace($search_array, $replace_array, $number);
    return $en_number;
  }
?>
~~~         




#  Convert lot of number English to Bangla      
~~~php
<?php
function convert ($n){
  
    $search_array = array("1", "2", "3", "4", "5", "6", "7", "8", "9", "0");
    $replace_array= array("১", "২", "৩", "৪", "৫", "৬", "৭", "৮", "৯", "০");
    $number = str_replace( $search_array,$replace_array, $n);
    
    
    return $number;
}
$all_number =[123, 345, 344, 333, 444];


$number = array_map("convert",$all_number );
$number =implode(',', $number);
echo $number;
?>
~~~
