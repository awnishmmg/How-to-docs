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
