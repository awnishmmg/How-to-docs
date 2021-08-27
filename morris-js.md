# Working with Morris.js Donuts Charts.

### Prepare the dataSet From the database ###

```

$pieChartsData = [];

		foreach ($sms_count_data as $key => $data_xy) {
			foreach ($data_xy as $label => $value) {
				$pieChartsData[] = [
					'label' => $label,
					'value' => $value,
				];
			}
		}
// prx($pieChartsData);

```


```
if(data.length){

Morris.Donut({
  element: id,
  data:data,
  dataLabels:true,

  colors:['yellow','red','green','blue','orange'],

  resize:true,
  formatter:function(y,data){
    return y;
  },

});

}else{
  $('#'+id).append('<label class="no-data-label">Sorry No Data Found!</label>');
     }
 
 ```
  
