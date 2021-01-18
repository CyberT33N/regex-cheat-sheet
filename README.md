# regex-cheat-sheet
Regex Cheat Sheet with the most needed stuff..





## Match word with numbers and dash
```javascript
let regex = /([a-z0-9-]+)/gmi;
```

<br><br>

## Match everything except specific character
```javascript
// match everything except =
let regex = /[^=]*/gmi;
```

<br><br>

## Dynamic change regex
```javascript
let regex = /^[\S\s]{1,300}([a-z0-9?!] |$)/gmi;
let trimmedString = $(this).html().match( regex );
```



<br><br>


 _____________________________________________________
 _____________________________________________________


<br />
<br />

# Numbers

## match numbers with or without commas
```javascript
/\d+([\d,]?\d)*(\.\d+)?/gmi
```


<br />
<br />


 _____________________________________________________
 _____________________________________________________


<br />
<br />


## Match everything including new lines
```javascript
// method 1
/[\S\s]/gmi

// method 2
/(?s:.)/gmi
```

## Replace all white spaces
```javascript
/\s\s+/gmi
```  

## Match everything without white space
```javascript
/[^\s]+/gmi
```  




## Remove all special Characters
```javascript
/[^a-zA-Z0-9 ]/gmi
```  



## Match space after specific amount of characters including new lines
```javascript
/^[\S\s]{1,200}( |$)/gmi
```  



## e-mail verification
```javascript
/(?:[a-z0-9!#$%&'*+/=?^_`{|}~-]+(?:\.[a-z0-9!#$%&'*+/=?^_`{|}~-]+)*|"(?:[\x01-\x08\x0b\x0c\x0e-\x1f\x21\x23-\x5b\x5d-\x7f]|\\[\x01-\x09\x0b\x0c\x0e-\x7f])*")@(?:(?:[a-z0-9](?:[a-z0-9-]*[a-z0-9])?\.)+[a-z0-9](?:[a-z0-9-]*[a-z0-9])?|\[(?:(?:(2(5[0-5]|[0-4][0-9])|1[0-9][0-9]|[1-9]?[0-9]))\.){3}(?:(2(5[0-5]|[0-4][0-9])|1[0-9][0-9]|[1-9]?[0-9])|[a-z0-9-]*[a-z0-9]:(?:[\x01-\x08\x0b\x0c\x0e-\x1f\x21-\x5a\x53-\x7f]|\\[\x01-\x09\x0b\x0c\x0e-\x7f])+)\])
/gmi
```  
