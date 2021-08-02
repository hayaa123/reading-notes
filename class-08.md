# CSS layout 

## positioning 

1- buildig blocks

- block element --> takes the whole block in html 
- inline element --> takes as its content takes and continuou after te privious element directly 

2- containing element : which mean a block inide a block , we can control this by :

- positional schemes

```

position : static --> every block element appeares in new line 
position : relative --> shifting the element from were it should be
position : absolute -->position the element in relation to its parent block + move as users scroll up and down the page
    
```

- box offset 

```

    position : fixed --> form of absolute positioning + positioning in relatio to the browser
    position : float --> allows you to take element out of its normal flow 

```

3- layout types 

- fixed  ---> the design dose not change when decrease or increase the size of browser

- liquid --> stretch and contract with the browser size

4- grids 

we can use grid to design a more flexable designs 

```

    display : grid

```
we can identify how many columns we want in one row and the ratios between them and also we can nest grids

![cheatsheet](https://res.cloudinary.com/practicaldev/image/fetch/s--X30jomsg--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://github.com/simonpaix/images/blob/main/blog/LearnPine_Grid_CheatSheet.png%3Fraw%3Dtrue)