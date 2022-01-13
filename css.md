# css

### Units

```css
div {
    width: 10px;
    width: 10%; /* 10% of the parent element */
    width: 10vw; /* 10% of the entire screen */
    width: 10rem; /* 10 x the font-size of the html element */
}
```
### Responsive Sizing

```css
div{
        /* mobile */
    html {
        font-size: 14px;
    }
    /* tablet */
    @media only screen and (min-width: 480px) {
        html {
            font-size: 16px;
        }
    }
    /* desktop */
    @media only screen and (min-width: 768px) {
        html {
            font-size: 18px;
        }
    }
    /* extra large */
    @media only screen and (min-width: 1024px) {
        html {
            font-size: 20px;
        }
    }

 .logo{
    height:3rem;
    width:3rem;
    background: url(https://example.com/image.png);
    background-position: center;
    background-repeat: no-repeat;
    background-size: contain;
    }
}
```


### Flexbox

```css
div {
    display: flex;

    /* justify-content aligns flex items along the main (horizontal) axis */
    justify-content: flex-start; /* default, items are packed toward the start line */
    justify-content: flex-end; /* items are packed toward to end line */
    justify-content: center; /* items are centered along the line */
    justify-content: space-between; /* items are evenly distributed in the line; first item is on the start   line, last item on the end line */
    justify-content: space-around; /* tems are evenly distributed in the line with equal space around them */
    justify-content: space-evenly; /* items are distributed so that the spacing between any two adjacent alignment subjects, before the first alignment subject, and after the last alignment subject is the same */

    /* align-items aligns flex items along the cross (vertical) axis */
    align-content: flex-start; /* lines packed to the start of the container */
    align-content: flex-end; /* lines packed to the end of the container */
    align-content: center; /* lines packed to the center of the container */
    align-content: stretch; /* lines stretch to take up the remaining space */

    /* flex-direction defines the direction of the main axis */
    flex-direction: row; /* same as text direction (default) */
    flex-direction: row-reverse; /* opposite to text direction */
    flex-direction: column; /* same as row but top to bottom */
    flex-direction: column-reverse; /* same as row-reverse top to bottom */

    /* order specifies the order of the flex items */
    order: <integer>; /* ...-1, 0 (default), 1...) */

    /* align-self aligns a flex item along the cross axis, overriding the align-items value */
    align-self: flex-start;
    align-self: flex-end;
    align-self: center;
    align-self: baseline;
    align-self: stretch;

    /* flex-wrap specifies whether flex items are forced on a single line or can be wrapped on multiple lines */ 
    flex-wrap: nowrap; /* single-line which may cause the container to overflow (default) */
    flex-wrap: wrap; /* multi-lines, direction is defined by flex-direction */
    flex-wrap: wrap-reverse; /* multi-lines, opposite to direction defined by flex-direction */

    /* flex-flow is shorthand for flex-direction and flex-wrap */
    flex-flow: <flex-direction><flex-wrap>;

    /* align-content aligns a flex container's line within the flex container when there is extra space on the cross axis */
    align-content: flex-start;
    align-content: flex-end;
    align-content: center;
    align-content: space-between;
    align-content: space-around;
    align-content: space-evenly;
    align-content: stretch; /* default */
    
}
```
