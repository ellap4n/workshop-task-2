# workshop-task-2
the URL for this task is here: https://ellap4n.github.io/workshop-task-2/

## Idea
Because this workshop played with intervals, I wanted to make something that moved in a logical way but repeated itself once started. This led me to think about water drops. 
I needed the drop to copy itslef moving down to 'animate' it, but I also needed the moving drop to keep repeating at regular intervals. 

## Interval coding 
this was very difficult as there was two layers of interval I wanted to operate - one of the water drop moving down, and another of the recursive water drop. 
I couldn't quite figure out how to get multiple drops of water using two set interval functions, so it instead repeats itself when the water reaches the bottom.
This worked quite nicely and gives a sort of hallucinative effect which I thought is cooler than my actual idea. 

## Conditionals for speed
It was a bit boring to watch, and unatural by the laws of physics - I wanted someone to be able to be distracted by this for while - 
so I decided that I wanted the water to slowly speed up as it flowed down the screen as water does in real life, so I used IF conditonals based on the height of the water drop - it worked ! as the water reached the bottom, the height was then reset to 0.
This was the code for it:

```
  if (height < 100) {
    height += 3;
  } else if (height < 125) {
    height += 4
  } else if (height < 200) {
    height += 5
  } else if (height < 250) {
    height += 6
  } else if (height < 300) {
    height += 7
  } else if (height < 350) {
    height += 8
  } else if (height < 420) {
    height += 9
  } else if (height = 420) {
    height = 0;
  }
}
```


## Cue on command
Next, to use the setTimeout function, I coded so that the water would 'turn on' when the mouse was clicked. as a function would have to be called, I put the falling interval into a new 'drop' function so that this interval was triggered when the mouse was clicked.
![Screenshot 2025-01-28 004358](https://github.com/user-attachments/assets/64690416-76bc-4f98-806b-0cafefb85d30)

## Finishing and Next steps
I chose colours that were quite minimalistic so the movement was the main focus of the page. 
I would like to eventually figure out how to make water flow simultaneously or have two drops flowing at the same time, maybe even create a splash at the bottom of the page. 
It would also be cool if the page started to slowly 'fill' with water.
