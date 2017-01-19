# learn-flexbox
Learning flexbox

## LINKS
- http://caniuse.com/#feat=flexbox
- https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Using_CSS_flexible_boxes
- https://css-tricks.com/snippets/css/a-guide-to-flexbox/
- http://flexboxfroggy.com/
- http://www.flexboxdefense.com/

## CSS PROPERTIES
### Parent
- **display: FLEX** Used to align _child elements_
```css
parentTarget{
  display: flex | inline-flex;;
}
```
- **align-items: option** _Align_ content in _container_
```css
parentTarget{
  align-items:  flex-start | flex-end | baseline | center | stretch | ;
}
```
- **justify-content: option** _Control_  **space** in _content_
  - **space-between** | _Between_ elements
  - **space-around** | _Around_ elements
```css
parentTarget{
  justify-content: space-between | space-around | flex-end | flex-start;
}
```
- **flex-direction: option** | _Direction_ flex work(_row column_)
```css
parentTarget{
  flex-direction: column | row | column-reverse | row-reverse;
}
```
- **flex-wrap: option** | _Wrap_ when _your size_ **is more** size the _your father_
```css
parentTarget{
  flex-wrap: nowrap | wrap | wrap-reverse;
}
```
- **flex-flow: direction wrap** | _Equal_ **flex-direction** and **flex-wrap**
```css
parentTarget{
  flex-flow: column wrap;
}
```



### Children
- **order** | Change _order_ element in _view_
```css
childrenElement{
  order: -1;
}
```
- **flex-grow: option** | _Get_ extra space, and modify your size **GROW UP**
```css
childrenTarget{
  flex-grow: 1;
}
```
- **flex-shrink: option** | _Get_ extra space, and modify your size _for_ **SHRINK**
```css
childrenTarget{
  flex-shrink: 2;
}
```
- **flex: grow shrink basis** | _Equal_ **flex-grow**, **flex-shrink** and **flex-basis**
```css
childrenTarget{
  flex: 0 1 25%;
}
```
- **flex-basis: value** | _Equal_ **witdh:**


## Parent and Children




## HTML USE
- **Find parent** of _elements_
```html
<div>
  <element />
  <element />
</div>
```


## OBSERVATIONS
- Who i want align?
  - **GET** your **parent**
- **justify-content** _only work if have space remaining_
- **display flex**
  - _All_ **children** win _same size_.
- **space-around space-between** is _bad_ for **grids**
- **MAIN AXIS** _horizontal_
  - **justify-content**
- **CROSS AXIS** _vertical_
  - **align-items**
- **flex-direction** _CHANGE_ the **MAIN AXIS**
- **order** have _0_ value with _default_
- **flex-shrink**: 0; | _DON't MODIFY SIZE_
