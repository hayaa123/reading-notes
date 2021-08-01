# Html tables 
 
+ we can use html table by using the `<table>` tag  
+ tables have tables rows and we can add it by using `<tr>` tag
+ table row contains data , we can add it by writing `td` tag 
+ we can define the head cells br writing `<hr>`
+ we can add head and foot and body for the table using  `<thead>`  ,`<tfoot>` ,`<tbody>`
+ we can add attribute to the tables rows or columns called span `rowspan` , `colspan` wich merge 2 rows or 2 cols together

```
<table>
<th>
<td>content of a head cell</td>
</th>

<tr>
<td>content of a table cell</td>
</tr>

</table>
```

# Functions, Methods, and Objects in JS 

we can add functions and methods to object by adding a property for it 

```
const object_name = { 
    property1 : value ,           ---> // we can call this outside the object by using method object_name.property1
    property2 : 0 ,               ---> // make sure that you add comma after each object key:value pair
    get_property2_function : function (){          ---> // we can add a function in the object 
        this.property2 = value            ---> //we should use this to refer to the element inside the object + we can assign values to     properties using this organized way
    }
}
```
