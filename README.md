# PyGame-Intro

This project shows the basic functionality of `Pygame` where I will show different things of how to create main screen, manage FPS, import game characters and basic movement

## Requirements

You only need to install `Pygame` and you can install it using 

```
pip install pygame
```

or you can just download the project and install the requirements using `requirements.txt` by using the command

```
pip install -r requirements.txt
```

## Basics

#### Main Screen

First we will draw the main screen and we will define `WIDTH, HEIGHT` of the screen in pixels and also define `COLOR` which takes a tuple as an input 


```python
import pygame 

WIDTH, HEIGHT = 900, 500
COLOR = (100, 125, 180)
```

and then we use `pygame.display` to display our main window

```python
WIN = pygame.display.set_mode((WIDTH, HEIGHT))
```

Now, we will make a function and name it `draw_window`, here we will fill our main window with color that we define earlier and update the display. One important thing
to notice is that everytime we draw something whether its window  or some shapes or assets on window we have to update the the display to apply changes.

```python
def draw_window():
    WIN.fill(COLOR)
    pygame.display.update()
```

Now we just call this function in our `main` function in a while loop and make it run for indefinite time by using a boolean `run`

```python
def main():
  run = True
  while run:
    draw_window()
if __name__ == '__main__':
    main()
```















