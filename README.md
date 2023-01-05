house price prediction 
<!DOCTYPE html>
<html >
<!--From https://codepen.io/frytyler/pen/EGdtg-->
<head>
  <meta charset="UTF-8">
  <title>House price prediction</title>
  <link href='https://fonts.googleapis.com/css?family=Pacifico' rel='stylesheet' type='text/css'>
<link href='https://fonts.googleapis.com/css?family=Arimo' rel='stylesheet' type='text/css'>
<link href='https://fonts.googleapis.com/css?family=Hind:300' rel='stylesheet' type='text/css'>
<link href='https://fonts.googleapis.com/css?family=Open+Sans+Condensed:300' rel='stylesheet' type='text/css'>

  
</head>

<body>
 <div class="login">
	<h1>House price  Prediction</h1>

     <!-- Main Input For Receiving Query to our ML -->
    <form action="{{ url_for('predict')}}"method="post">
      <input type="text" name="CRIM" placeholder="CRIM" required="required" /><br>
    	<input type="text" name="ZN" placeholder="ZN" required="required" /><br>
        <input type="text" name="INDUS" placeholder="INDUS" required="required" /><br>
        <input type="text" name="CHAS" placeholder="CHAS" required="required" /><br>
        <input type="text" name="NOX" placeholder="NOX" required="required" /><br>
        <input type="text" name="RM" placeholder="RM" required="required" /><br>
        <input type="text" name="AGE" placeholder="AGE" required="required" /><br>
        <input type="text" name="DIS" placeholder="DIS" required="required" /><br>
        <input type="text" name="RAD" placeholder="RAD" required="required" /><br>
        <input type="text" name="TAX" placeholder="TAX" required="required" /><br>
        <input type="text" name="PTRATIO" placeholder="PTRATIO" required="required" /><br>
        <input type="text" name="B" placeholder="B" required="required" /><br>
        <input type="text" name="LSTAT" placeholder="LSTAT" required="required" /><br>


        <button type="submit" class="btn btn-primary btn-block btn-large">Predict</button>
    </form>

   <br>
   <br>
  
   
 </div>
 {{prediction_text}}

</body>
</html>
