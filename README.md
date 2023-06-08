# To-do-List
Manage your daily tasks with this awesome to-do list :clipboard:<br></br>
<img src="https://github.com/Maruku98/To-do-List/assets/133391272/d1990a82-db80-4932-8e76-77ac2eac361d" width="600">

## Overview
This is my second React project. Even though it may seem such a simple project, I believe it was an excellent opportunity to further learn more basic concepts about React hooks and state.<br></br>
My to-do list features a `regex` non-ASCII characters detector, a duplicate task detector, and much more!

## PROGRAMMING LANGUAGES USED
- HTML5
- CSS3
- JavaScript ES6
- React :electron:

## FEATURES
### Overall behavior
Users are expected to type a to-do task in the provided input. Once written, tasks can be added whether by clicking the button with the mouse or the "Enter" key on the keyboard.  
Considering that, the program features some user input limitations:  
- Non-ASCII characters like "ñ" or accents are not allowed. A message letting the users know about this will be displayed upon typing one in the input. Thus, the application detects whether the input contains, at least, one non-ASCII character.  
This is achieved with `regex` `/[^\x00-\x7F]/`.
- The warning message is shown or hidden via conditional rendering.
- Repeated tasks are not allowed. Users will be alerted that the task is already in the list, and that task won't be added to the list.
- Empty inputs or inputs containing no characters (like white spaces only) are not accepted. Naturally, tasks containing any non-ASCII character won't be added to the list either.
- Users can remove tasks individually by clicking the red "X" to the right of the task.
- A reset button is provided to remove all tasks at once.
- A clear button is also provided to clear input text.
