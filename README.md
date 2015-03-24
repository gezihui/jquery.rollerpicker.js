# jquery.rollerpicker.js
a fun rollerpicker for short and simple pulldown menu

## How to use
include: 
<script type="text/javascript" src="js/jquery.rollerpicker.js"></script>
<link rel="stylesheet" href="css/rollerPicker.css" />

HTML:
<div class="rollerPicker" id="myPicker"></div>

JS:
$(document).ready(function()
  {
   var box = $('#myPicker');
    box.rollerpicker({values: ["0", "1", "2", "3", "4", "5", "6", "7", "8", "9", "10", "11"],
    icons: ["images/shape0.png", "images/shape0.png", "images/shape0.png", "images/shape0.png",
    "images/shape0.png", "images/shape0.png", "images/shape0.png", "images/shape0.png",
    "images/shape0.png", "images/shape0.png", "images/shape0.png", "images/shape11.png"]});
  
  //set initial value
  box.data("plugin_rollerpicker").setPick(1, "");
  
  //binding on change
  box.bind("change", function(evt, val){});
});

