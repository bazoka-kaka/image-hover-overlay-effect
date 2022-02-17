# Image Hover Overlay Effect

things to note:
- transition<br>
we have to use transition to make an animation from normal state to hover state

e.g:
```
.element {
  opacity: 0;
  transition: opacity 0.25s;
}

.element:hover {
  opacity: 1;
}
```

- wildcard<br>
we have to use wildcard selector after the more than symbol 
to select all the elements inside an element

e.g:

index.html:
```
 <div class='element-container'>
  <div class='element1'></div>
  <div class='element2'></div>
 </div>
```
styles.css:
```
 .element > * {}
```

note:
this is gonna select element1 and element2

- image blur<br>
we have to use backdrop-filter: blur(); to make blurring effect

e.g
```
.image {
  backdrop-filter: blur(5px);
}
```

note:
this is gonna work on most websites, but not all
