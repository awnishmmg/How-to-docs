# Working with Imagick Function to Increase the Resolution
https://stackoverflow.com/questions/13656631/how-to-increase-image-resolution-in-imagemagick-in-php
# Working with Imagick Function to Convert pdf to image
https://stackoverflow.com/questions/57671994/while-creating-image-from-pdf-using-imagick-i-get-the-following-error-can-anyb

# Magnipopup for the Image Gallery View
## Documentation Link 
https://dimsemenov.com/plugins/magnific-popup/documentation.html
## Code Snippet

```
<!DOCTYPE html>
<html lang="en">
<head>
  <title>Bootstrap Example</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">

  <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
  
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/magnific-popup.js/1.1.0/magnific-popup.min.css" integrity="sha512-+EoPw+Fiwh6eSeRK7zwIKG2MA8i3rV/DGa3tdttQGgWyatG/SkncT53KHQaS5Jh9MNOT3dmFL0FjTY08And/Cw==" crossorigin="anonymous" referrerpolicy="no-referrer" />
  
</head>
<body>

<div class="jumbotron text-center">
  <h1>Gallery View</h1>
  <p>Click On the Image</p> 
</div>
  
<div class="container">
  <div class="row">
      <div class="gallery-container">
            <div class="col-md-2">
                <a href="https://images.unsplash.com/photo-1626160200758-71b8bf10d34f?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1534&q=80" target="_blank">
                  <img src="https://images.unsplash.com/photo-1626160200758-71b8bf10d34f?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1534&q=80" class="image-fluid">
                </a>
          </div>
          <div class="col-md-2">
                <a href="https://images.unsplash.com/photo-1626197219310-8be29c1316be?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1500&q=80" target="_blank">
                  <img src="https://images.unsplash.com/photo-1626197219310-8be29c1316be?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1500&q=80">
                </a>
          </div>
     </div>
  </div>
</div>

</body>

<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.16.0/umd/popper.min.js"></script>
  <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>
  
  <script src="https://cdnjs.cloudflare.com/ajax/libs/magnific-popup.js/1.1.0/jquery.magnific-popup.min.js" integrity="sha512-IsNh5E3eYy3tr/JiX2Yx4vsCujtkhwl7SLqgnwLNgf04Hrt9BT9SXlLlZlWx+OK4ndzAoALhsMNcCmkggjZB1w==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>

  <script type="text/javascript">
    // Important Line 
    $(document).ready(function(){

        $(".gallery-container").magnificPopup({  // Initialise the MagnificPopup
          delegate: 'a',
          type:'image',
          gallery: {
            enabled: true   //Enable the Gallery Mode
             },
        });

        //Automatic Open the First Image 
        $(".gallery-container a").click();  // Auto pop-up
    });

  </script>
</html>




```





# Best Way to Connect with Mysqli
```
try
{	
	mysqli_report(MYSQLI_REPORT_ERROR | MYSQLI_REPORT_STRICT);
    if($con=mysqli_connect($hostname,$username,$password,$dbname)){
   //do something
    }
    else
    {
        throw new Exception;
    }
}
catch(Exception $e)
{
    echo $e->getMessage();
}

```

# Handling the File 
https://stackoverflow.com/questions/19280901/javascript-upload-and-parse-file-on-fly

# Best Match case for mobile numbers
https://stackoverflow.com/questions/3813195/regular-expression-for-indian-mobile-numbers/3813226#3813226

# Replace Single or Double Qoutes from data

https://stackoverflow.com/questions/14743812/how-to-use-str-replace-to-replace-single-and-double-quotes

# Break Large File into Chunks
https://stackoverflow.com/questions/4694394/break-a-large-file-into-many-smaller-files-with-php

# How to create Custom Login System Without Authentication Module
https://codingdriver.com/laravel-custom-authentication-tutorial-with-example.html

# Important Laravel Command 
```
1. php artisan inspire
2. php artisan migrate --pretend --ansi > dump.sql [Overwrite]
3. php artisan migrate --pretend --ansi >> dump.sql [Append Mode]
4. echo <output-string> > <output.txt file> [Overwrite Mode]
   echo <output-string> >> <output.txt file> [Overwrite Mode]
```

# How-to-docs
Here I Add the Important Link of Stack Over Flow

# How to Dynamically Added the Links of Header Css and Jss in CodeIgnitor using Custom Config Files
https://stackoverflow.com/questions/39042472/dynamically-add-javascript-and-css-files-in-codeigniter-head-section
https://jamshidhashimi.com/2013/04/12/dynamically-add-javascript-and-css-files-in-codeigniter-header-page/

# How to Add Custom date picker using jquery ui
https://tamble.github.io/jquery-ui-daterangepicker/

# Best PlugIn to Handle Multiple File Uploaded using Progress Bar in Built in JQuery UI
http://hayageek.com/docs/jquery-upload-file.php#multi

# Self Executing function is best Technique for Running Ajax Script inside loop
https://stackoverflow.com/questions/21819905/jquery-ajax-calls-in-for-loop
```
$(document).ready(function(){
   var entity_class =  document.getElementsByClassName("dynamic_entityID");
   var entity_id = [];
   for(var i=0;i<entity_class.length;i++){
        entity_id.push($(entity_class[i]).val());
   }
   
   for(var j=0;j<entity_id.length;j++){
       
      (function(j){
          $.ajax({
            url:site_url+"ndlc-complaints/fetch_senderId/"+entity_id[j],
            type:"GET",
             success:function(response){
              if(response.response_code==200 && response.status==true){
                  console.log(response);
                    // $(".dynamic_sender_"+j).html("");
                    console.log($(".dynamic_sender_"+j));
                    // $(".dynamic_entityID"+j).css("border","");
                    $(".dynamic_sender_"+j).append('<option value="">Select</option>');
                    $(response.response_data).each(function(index,sender){
                        $(".dynamic_sender_"+j).append('<option value="'+sender.id+'">'+sender.header_name+'</option>');
                    });
                    
                    $(".dynamic_sender_"+j).find("option[value='"+ $(".dynamic_sender_"+j).attr('title')+"']").attr("selected","selected");
                
                    
              }else{
                  
                   $(".dynamic_sender_"+j).html('<option value="">Select</option>');
                   
                
                   
              }
              
           
          }
           
   });
          
      })(j);
      
       
       
       
   }//end of Ajax Request 
   
   
});
```
# Crud using JSON
https://stackoverflow.com/questions/38301457/php-crud-json-file-instead-of-a-database-like-mysql

# Function to write Data in local Storage

https://stackoverflow.com/questions/16083919/push-json-objects-to-array-in-localstorage

```
function SaveDataToLocalStorage(data)
{
    var a = [];
    // Parse the serialized data back into an aray of objects
    a = JSON.parse(localStorage.getItem('session')) || [];
    // Push the new data (whether it be an object or anything else) onto the array
    a.push(data);
    // Alert the array value
    alert(a);  // Should be something like [Object array]
    // Re-serialize the array back into a string and store it in localStorage
    localStorage.setItem('session', JSON.stringify(a));
}
```
