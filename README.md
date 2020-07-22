
# stylight
A mini utility scss library based on bootstrap from [@censodev](https://github.com/censodev) with love

## Theme 
> Base theme color
> Can be customized in _theme.scss
```scss
"white":        #ffffff,
"black":        #000000,
"transparent":  transparent,
"dark":         #343a40,
"primary":      #3f51b5,
"secondary":    #6c757d,
"link":         #000000, 
"faded":        rgba(0, 0, 0, 0.54),
"accent":       #ff4081,
```

## Utilities
### Background
> Background color
```scss
.bg-#{$theme}
```

```html
<div class="bg-primary">...</div>
<div class="bg-transparent">...</div>
```

### Border
> Aspect
```
top, bottom, left, right
```
> Border
```scss
.border-#{$aspect}
.border-#{$aspect}-0
```
> Border radius
```scss
.rounded-#{$aspect}
.rounded-#{$aspect}-0
```
> Border color
```scss
.border-#{$theme}
```
```html
<div class="border">...</div>
<div class="border-top">...</div>

<div class="border-0">...</div>
<div class="border-top-0">...</div>

<div class="rounded">...</div>
<div class="rounded-top">...</div>

<div class="rounded-0">...</div>
<div class="rounded-top-0">...</div>

<div class="border-primary">...</div>
<div class="border-transparent">...</div>
```

### Display
```scss
.d-none  		{  display:  none  !important;  }
.d-inline  		{  display:  inline  !important;  }
.d-inline-block		{  display:  inline-block  !important;  }
.d-block  		{  display:  block  !important;  }
.d-table  		{  display:  table  !important;  }
.d-table-row		{  display:  table-row  !important;  }
.d-table-cell		{  display:  table-cell  !important;  }
.d-flex  			{  display:  flex  !important;  }
.d-inline-flex		{  display:  inline-flex  !important;  }
```

### Flex
> Direction
```scss
.flex-row  		{  flex-direction:  row  !important;  }
.flex-column  		{  flex-direction:  column  !important;  }
.flex-row-reverse  	{  flex-direction:  row-reverse  !important;  }
.flex-column-reverse	{  flex-direction:  column-reverse  !important;  }
```
> Wrap
```scss
.flex-wrap  		{  flex-wrap:  wrap  !important;  }
.flex-nowrap  		{  flex-wrap:  nowrap  !important;  }
.flex-wrap-reverse  	{  flex-wrap:  wrap-reverse  !important;  }
```
> Justify content
```scss
.justify-content-start  	{  justify-content:  flex-start  !important;  }
.justify-content-end  		{  justify-content:  flex-end  !important;  }
.justify-content-center  	{  justify-content:  center  !important;  }
.justify-content-between  	{  justify-content:  space-between  !important;  }
.justify-content-around  	{  justify-content:  space-around  !important;  }
```
> Align items
```scss
.align-items-start  	{  align-items:  flex-start  !important;  }
.align-items-end	{  align-items:  flex-end  !important;  }
.align-items-center  	{  align-items:  center  !important;  }
.align-items-baseline  	{  align-items:  baseline  !important;  }
.align-items-stretch  	{  align-items:  stretch  !important;  }
```
> Align content
```scss
.align-content-start  	{  align-content:  flex-start  !important;  }
.align-content-end  	{  align-content:  flex-end  !important;  }
.align-content-center  	{  align-content:  center  !important;  }
.align-content-between  {  align-content:  space-between  !important;  }
.align-content-around  	{  align-content:  space-around  !important;  }
.align-content-stretch  {  align-content:  stretch  !important;  }
```
> Align self
```scss
.align-self-auto	{  align-self:  auto  !important;  }
.align-self-start	{  align-self:  flex-start  !important;  }
.align-self-end		{  align-self:  flex-end  !important;  }
.align-self-center  	{  align-self:  center  !important;  }
.align-self-baseline  	{  align-self:  baseline  !important;  }
.align-self-stretch  	{  align-self:  stretch  !important;  }
```
> Grow and shrink
```scss
.flex-grow-0  	{  flex-grow:  	0;  }
.flex-grow-1  	{  flex-grow:  	1;  }
.flex-shrink-0  {  flex-shrink:	0;  }
.flex-shrink-1  {  flex-shrink:	1;  }
```
> Magic margin
> > prefix: m ~ margin
> postfix: null, x, y, t, b, l, r ~ all aspects, left-right, top-bottom, top, bottom, left, right
```html
<div class="d-flex">
	<div class="ml-auto">margin-left: auto</div>
</div>
```

### Position
> Position
```
static, relative, absolute, fixed, stickey
```
> Common
```scss
.position-#{$position}
```
```html
<div class="position-static">...</div>
<div class="position-relative">...</div>
<div class="position-absolute">...</div>
<div class="position-fixed">...</div>
<div class="position-sticky">...</div>
```
> Fixed top/bottom
>> Position an element at the top/bottom of the viewport, from edge to edge
```html
<div class="fixed-top">...</div>
<div class="fixed-bottom">...</div>
```
> Sticky top
>> Position an element at the top of the viewport, from edge to edge, but only after scrolling past it
```html
<div class="sticky-top">...</div>
```

### Sizing
> Size in [5%, 100%] with step 5%
```scss
.w-#{$size}
.h-#{$size}
```
> Max size
```scss
.mw-#{$size}
.mh-#{$size}
```

```html
<div class="w-10">width 10%</div>
<div class="h-10">height 10%</div>

<div class="mw-10">max width 10%</div>
<div class="mh-10">max height 10%</div>
```

### Spacing
> prefix: m, p ~ margin, padding
> postfix: null, x, y, t, b, l, r ~ all aspects, left-right, top-bottom, top, bottom, left, right
```scss
0: 0,
1: 0.25 rem,
2: 0.5 rem,
3: 1 rem,
4: 1.5 rem,
5: 3 rem
```
```html
<div class="m-3">margin: 1rem 1rem</div>
<div class="ml-5">margin-left: 3rem</div>
<div class="py-5">padding-top: 3rem; padding-bottom: 3rem</div>
```

### Text
> Font size
```scss
0: 0,
1: 0.5 rem,
2: 0.75 rem,
3: 1 rem,
4: 1.25 rem,
5: 1.5 rem
```
```html
<span class="font-size-4">font-size: 1.25rem</span>
```
> Alignment
```scss
.text-justify  	{  text-align:  justify  !important;  }
.text-left  	{  text-align:  left  !important;  }
.text-right  	{  text-align:  right  !important;  }
.text-center  	{  text-align:  center  !important;  }
```
> Wrap, Truncate, Break
```scss
.text-wrap  	{  white-space:	  normal  !important;  }
.text-nowrap  	{  white-space:	  nowrap  !important;  }
.text-truncate  {  overflow:	  hidden;
		   text-overflow: ellipsis;
		   white-space:	  nowrap;  }
.text-break  	{  word-wrap:  break-word  !important;  }
```
> Transformation
```scss
.text-lowercase		{  text-transform:  lowercase  !important;  }
.text-uppercase		{  text-transform:  uppercase  !important;  }
.text-capitalize	{  text-transform:  capitalize  !important;  }
```
> Weight and Italic
```scss
.font-weight-light  	{  font-weight: 300 !important;  }
.font-weight-normal  	{  font-weight: 400 !important;  }
.font-weight-bold  	{  font-weight: 700 !important;  }
.font-italic  		{  font-style:  italic  !important;  }
```
> Remove underline on a <a>link</a>
```html
<a href="#" class="text-decoration-none">link</a>
```
> Text color
```scss
.text-#{$theme}
```
```html
<span class="text-primary">...</span>
<span class="text-secondary">...</span>
```

## Media
> Magic image
```scss
.object-fit-cover  { object-fit:  cover; }
```

## Scroll
> Hide scroll
```scss
.scroll-hidden  {
	-ms-overflow-style:  none;  /* IE and Edge */
	scrollbar-width:  none;  /* Firefox */

	/* Hide scrollbar for Chrome, Safari and Opera */
	&::-webkit-scrollbar  {
		display:  none;
	}
}
```
