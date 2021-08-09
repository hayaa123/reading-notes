# Storage HTML5 

- store in the user browser (browser independent)
-

## 3 ways to store data

1) local storage 
-  store larger amount of data 
- supported by HTML5
- accessible in any window (all tabs) 
- never removed until the user removed it

```
// Store
localStorage.setItem("lastname", "Smith");

// Retrieve
document.getElementById("result").innerHTML = localStorage.getItem("lastname");
```

2) session storage 
- store large amount of data
- supported by HTML5
- accessible in the same tab
- removes when close tab

```
if (sessionStorage.clickcount) {
  sessionStorage.clickcount = Number(sessionStorage.clickcount) + 1;
} else {
  sessionStorage.clickcount = 1;
}
document.getElementById("result").innerHTML = "You have clicked the button " +
sessionStorage.clickcount + " time(s) in this session.";
```

3) cookies
- store small amount of data
- supported in html4 and html5 
- accessible in any window (all tabs) 
- set when it will be expired


I finished this reading using [w3school](https://www.w3schools.com/html/html5_webstorage.asp)
and [this vedio](https://www.youtube.com/watch?v=GihQAC1I39Q)