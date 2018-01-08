# metricapp
Simple metric conversion app that does miles to kilometers to centimeters.
<!DOCTYPE>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    py
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0-alpha.6/css/bootstrap.min.css" integrity="sha384-rwoIResjU2yc3z8GV/NPeZWAv56rSmLldC3R/AZzGRnGxQQKnKkoFVhFQhNUwEyJ" crossorigin="anonymous">
    
    <style>
        body{
            margin-top:70px;
            background:#333;
            color:#fff;
        }
    </style>
    <title>Metric App</title>
    
    </head>
<body>
    <div class="container">
  <div class="row">
    <div class="col-md-6 offset-md-3">
      <h1 class="display-4 text-center mb-3">Metric App</h1>
      <form>
        <div class="form-group">
          <input id="milesInput" type="number" class="form-control form-control-lg" placeholder="Enter Miles...">
        </div>
      </form>
      <div id="output">
        <div class="card card-danger mb-2">
          <div class="card-block">
            <h4>Kilometers:</h4>
            <div id="kgOutput"></div>
          </div>
        </div>

        <div class="card card-warning mb-2">
          <div class="card-block">
            <h4>Meters:</h4>
            <div id="mtOutput"></div>
          </div>
        </div>

        <div class="card card-success mb-2">
          <div class="card-block">
            <h4>Centimeters:</h4>
            <div id="centiOutput"></div>
          </div>
        </div>
          
          
      </div>
    </div>
  </div>
</div>
    
            
                <script>
                    
                  
        
        document.getElementById("milesInput").addEventListener("input",function(e){
           
            document.getElementById("output").style.visibility = "visible";
            
            let miles = e.target.value;
            document.getElementById("kgOutput").innerHTML = miles  * 1.60934;
            
            document.getElementById("mtOutput").innerHTML = miles * 1000;
            
            document.getElementById("centiOutput").innerHTML = miles * 160394;
            
            
        });
                                                               
        
        
        
        </script>
            
            
            
        
            
        
    
    
    
    </body>
</html>
