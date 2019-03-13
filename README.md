# Animate Numbers

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>Animate Numbers</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/4.3.1/css/bootstrap-grid.min.css">
</head>
<body>

  <div class="animate-numbers">
    <div class="container">
      <div class="row">
  
        <div class="col-lg-3">
          <div class="animate-numbers__item">
            <span id="fun-level1">0</span>
            <div class="number-title">Satisfied customers</div>
          </div>
        </div>

        <div class="col-lg-3">
          <div class="animate-numbers__item">
            <span id="fun-level2">0</span>
            <div class="number-title">Successful projects</div>
          </div>
        </div>

        <div class="col-lg-3">
          <div class="animate-numbers__item">
            <span id="fun-level3">0</span>
            <div class="number-title">Reliable partners</div>
          </div>
        </div>

        <div class="col-lg-3">
          <div class="animate-numbers__item">
            <span id="fun-level4">0</span>
            <div class="number-title">Contracts</div>
          </div>
        </div>
  
      </div>
    </div>
  </div>

  <script src="http://code.jquery.com/jquery-3.3.1.min.js"></script>
  <script src="libs/jquery.waypoints.min.js"></script>
  <script src="libs/jquery.animateNumber.min.js"></script>
  <script >
    $(function(){

      $('#fun-level1').waypoint(function() { // waypoint offset 80%
    
        // animate numbers
        $('#fun-level1').animateNumber({ number: 1036 }, 5000);
        $('#fun-level2').animateNumber({ number: 3047}, 5000);
        $('#fun-level3').animateNumber({ number: 1002 }, 5000);
        $('#fun-level4').animateNumber({ number: 2374 }, 5000);
    
        this.destroy();
    
      }, {
        offset: '80%'
      }); // waypoint offset 80%

    });
  </script>
  
</body>
</html>
```
