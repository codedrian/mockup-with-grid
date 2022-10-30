## Mockup with Grid

### What I've learned today:
- In this activity I've learned how to get the article cards automatically fit as the windows is adjusted. To accomplish this, I used 

```
grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); 
``` 
So what's going on here? The ```auto-fit``` will return the highest positive integer without overflowing the grid. For example, the size of the window is `500px` wide, the ```minmax()``` will return the highest values which is ```250px```. So, if our window is ```500px``` wide, the grid will render 2 columns and then resizes the columns by the value I allowed in the ```minmax()``` function which is ```1fr```. Through this, the columns automagically know how many will fit across without any media queries whatsoever. Cool, innit?
