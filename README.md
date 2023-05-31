# JSLimitCharacterTitle
JavaScript / jQuery Limit Character display in title or description 

```JS
// jQuery 

// Limit display title post 
let targetElem = jQuery('.title-class');
// from 0 to 10 instead of having large text 
// Default *like : Titlefghjaskklasjlasbdabsldkhalskdjakldhajsbjlashdlkasdhlaksdhlaksdhalksdhal
// Output *To : Titlefghjask
targetElem.text(targetElem.text().substring(0,10)) // .substring(0,10)+'...') // Output *To : Titlefghjask ...
```

```JS
// Pure JS 
var i;
var divs = document.getElementById('#your-div-id');
for(i=0;i<divs.length;i++) {
  if(divs[i].className == 'myclass') {
    divs[i].innerHTML = divs[i].innerHTML.substring(0,300);
  }
}
```

Source: https://stackoverflow.com/questions/19425555/maximum-amount-of-characters-in-a-div-paragraph-tag
