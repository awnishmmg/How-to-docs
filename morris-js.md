# Working with Morris.js Donuts Charts.

### Prepare the dataSet From the database ###

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
  
