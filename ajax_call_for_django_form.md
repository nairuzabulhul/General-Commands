











## HTML
```
<!DOCTYPE html>
<html>
<head>
    <title>WIZARD</title>
</head>

<body>
        
<form method="POST" action="#" id="theForm">
  
    <!--HIDDEN ID-->
    {% csrf_token %}
    <input type="hidden" id="id" name="id" value="">

    <div>
        <label for="first_name">First Name</label>
        <input type="text" name="first_name" id="first_name">
    </div>
    
    <div>
        <label for="lalast_name">Last Name</label>
        <input type="text" name="last_name" id="last_name">
    </div>
    
    <div>
        <label for="company_name">Company Name</label>
        <input type="text" name="company_name" id="company_name">
    </div>

    <button id="btnn">Submit</button>
    
</form>

<script src='https://cdnjs.cloudflare.com/ajax/libs/jquery/2.1.3/jquery.min.js'></script>
<script src='https://maxcdn.bootstrapcdn.com/bootstrap/3.3.5/js/bootstrap.min.js'></script>
<script src='https://cdnjs.cloudflare.com/ajax/libs/1000hz-bootstrap-validator/0.9.0/validator.min.js'></script>
<script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/bootstrap-datepicker/1.4.1/js/bootstrap-datepicker.min.js"></script>
</body>
</html>

```



## JS script with AJAX CALL

```
<script type="text/javascript">
 $(document).ready(function(){
        
       var timeoutID;
    
        $('#theForm').on('input', function() {
            // clears window time out
            clearTimeout(timeoutID);
            timeoutID = setTimeout(saveToDB, 1000);
    
        });
    
    
        //Serialize the form to JSON object
        $.fn.serializeObject = function(){
                
            var jsonObject = {};
            var formSerializeArray = this.serializeArray(); //serialize the form
            
            // for every item in the serizalize array
            $.each(formSerializeArray, function() {
                  
                if (jsonObject[this.name] !== undefined) {
                        alert("UNDEFINED");
                } else {
                    jsonObject[this.name] =   this.value ;
                }
            });
            
            //reutrn full JSON object
            return jsonObject;
        
            console.log(jsonObject);
        };
    
    
        // Save to the db usign AJAX call
        function saveToDB() {
            
            var $form = $("#theForm");
            var formData = $form.serializeObject();
            var inputID = $("#id");
            // console.log(typeof(formData))
        
            // AJAX call
             $.ajax({
                // Call the "wizard_api_view" 
                url: 'api/wizard/',
                type: "POST",
                dataType:"json",
                data: formData, // serialize the form as JSON
                success: function (data) {
                    // If the data is posted, show success message
                    // var parsedData = JSON.parse(data);
                    // console.log(typeof(parsedData));
                    console.log('Successfully posted!', data); 
                    // console.log('Response data:', formData.id);
                    // console.log('OBJECT ID:', parsedData[0].pk)
                    // inputID.val(parsedData[0].pk); //capture POST request id
                },
                error: function (error) {
                    console.log("ERROR:", error);
                }
            });
        
        }
        
    });

</script>
 ```
 
 

