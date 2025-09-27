# Chess Game using Pygame

The source of this program is from the Youtube Tutorial
[Create Your Own Chess Game with Python and Pygame: Step-by-Step Tutorial!](https://www.youtube.com/watch?v=yeBOopkWqe0)

## How to Run this code
`` python3 main.py ``

## Changes and Bug fixes

### Black Knight

The PNG for Black Knight was not correct. Therefore, *black_knight.png* has been updated.

### The handling of 'Check' i.e. Fix bug regarding 'def is_check(color)'

The logic for whether a player was in 'check' needed fixing.

### The handling of 'Checkmate'

#### 'White'

After fixing the bugs regarding the handling of 'check',<br>
I tested the 'checkmate' functionality for WHITE using 

```
1. e4 e5
2. Qh5 Nc6
3. Bc4 Nf6
4. Qxf7#
```

This CheckMate is Demonstrated by this Video: [CHECKMATE in 4 Moves!](https://www.youtube.com/shorts/1Mn2Kb4QQe8)

When these moves are followed, 
the program correctly displays:<br>
**Checkmate! Black loses.**

The above is variation of what is known as **Scholar’s Mate.**

*What Is the Scholar’s Mate?*

```
Here are the annotations for a basic scholar’s mate:

1. e4 e5
2. Bc4 Nc6
3. Qh5 Nf6
4. Qxf7#
```
SOURCE: [What Is the Scholar’s Mate?](https://www.masterclass.com/articles/scholars-mate-explained)

#### 'Black'

Tested the 'checkmate' functionality for BLACK using **Fool's Mate**

```
Black can achieve checkmate in two moves against a significant blunder by White with the moves 
1. f3 e5 2. g4?? Qh4#.
This sequence is known as Fool's Mate and relies on White's extraordinary mistakes.  

Moves: 
f3: (White moves the f-pawn one square forward)
e5: (Black moves their e-pawn one square forward)
g4?? (White moves their g-pawn two squares forward, a huge mistake)
Qh4#: (Black moves their Queen to h4, delivering checkmate)
```

This CheckMate is Demonstrated by this Video: [Demonstrated by this Video Short: How To Win Chess in 2 Moves](https://www.youtube.com/shorts/4E9drlZ0Vns)

When these moves are followed, 
the program correctly displayed:<br>
**Checkmate! White loses.**

Note: there are variations of this kind of Fool's mate <br>
e.g. **1. f3 e6 2. g4?? Qh4#.**

## TODO

1. The chess move *En Passant* needs to be added
2. The chess move *Castling* needs to be added
3. This program allows a user to make a move which leaves their king in 'check'.<br>**This is not allowed in the [Rules of Chess](https://en.wikipedia.org/wiki/Rules_of_chess)**

## Miscellaneous

### Create an environment

```
# Windows
# You can also use `py -3 -m venv .venv`
python -m venv .venv
```

[SOURCE](https://code.visualstudio.com/docs/python/environment)
  