<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width">
  <title>JS Bin</title>
   <style>
     .bad {color:gray;
           text-decoration:line-through;
     }
  
  </style>
</head>
<body>
  
  <div class='work'>
     <input type="checkbox" class="box"> Встать 
  </div>
  <div class='work'>
    <input type="checkbox" class="box">Умыться
  </div>
  <div class='work'>
    <input type="checkbox" class="box">Покушать 
  </div>
  <div class='work'>
    <input type="checkbox" class="box">Собраться на работу
  </div>
   <script>
          
      var items = document.querySelectorAll('.work' )
      items.forEach(
        function (node) {
           node.addEventListener('click', 
             function() {
                this.classList.toggle('bad')
                this.children[0].checked = !this.children[0].checked;
              }
           )
           
        }
      ) 

     
   
      
      
      
        
      
     
  </script>
  
</body>
</html>  
