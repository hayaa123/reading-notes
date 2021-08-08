# Javascript Chart 

we can draw charts in js using Chat.js  we can import it using this script 

```
        <script src='Chart.min.js'></script>

```

we can draw line ,pie and bar chart using it  

to start draw chart we cal `canvus` tag in HTML which take hight and width attributes 

then we creat graph using JS 

```
var name = document.getElementById("name_id").getContext("2d");

new Chart(name).Bar(barData); -->  //for drawing bar chart 
```

and then add the bar charts data 

```
var chart = {
    labels :""
    datasets :[
        {
            fillColor :
            strokColor : 
            data : []
        },
        {
            fillColor :
            strokColor : 
            data : []
        }etc
    ]
}
```


# Drawing text 

first we should select element 

```
var ctx = document.getElementById('canvas').getContext('2d');
ctx.font =
ctx.fillText =
ctx.rextBaseline =
textAlign = 
direction =
```



