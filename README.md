# Real-Time-Sudoku-Solver-OpenCV-and-Keras
Solves a Sudoku puzzle under one second and overlays the solved puzzle on to the original image in real-time. 
This repo consists of Python code for solving sudoku puzzle using Deep Learning and OpenCV in real time(Live Camera).<br>
Main Reference: [Anh Minh Tran](https://www.youtube.com/watch?v=uUtw6Syic6A&list=LLwC_qd6q9vEqDaxU3KdSgPw&index=2&t=236s)

##### <div><img src="https://uxwing.com/wp-content/themes/uxwing/download/10-brands-and-social-media/linkedin-color.png" width="25" height="25"> Linkedin: https://www.linkedin.com/in/snehit-vaddi-73a814158/</div>
## Sample outputs from Custom YOLOv3 model
<img src="https://github.com/snehitvaddi/Real-Time-Sudoku-Solver-OpenCV-and-Keras/blob/master/output/output-gif.gif" width="400">

## Algorithim Used
In general Sudoku is solved using Backtracking approch, where it is a bruteforce approch.<br>
Here we are using **Greedy Best First Search approch**!! -> which an optimised version of Naive Back Tracking method ie; Chooses a cell with least number of possibilities to search next.

## How to Run!!
Step-1: Install all required libraries in `requirements.txt` or directly run `pip install -r requirements.txt`<br>
Step-2: Directly run all cells of `Sudoku testing.ipynb` file. It does all the imports by itself.<br>
Step-3: Nothing else, just get your Sudoku puzzle in front of your camera and solutions will be relayed over their respective positions.<br>
Step-2: To stop the camera, click 'Q' on keyboard.

## Note:
I already trained my keras model to predict digits. You can try your custom model to predict similarly!!

## References:
#### Algorithim:
For solving sudoku: https://norvig.com/sudoku.html<br>
Tech With Tim: https://www.youtube.com/watch?v=lK4N8E6uNr4
#### Theoretical:
Sudoku extraction from image: https://medium.com/@neshpatel/solving-sudoku-part-ii-9a7019d196a2 (with python code)
Solving Sudoku Part1: https://medium.com/@neshpatel/solving-sudoku-part-i-7c4bb3097aa7
Solving Sudoku Part2: https://medium.com/@neshpatel/solving-sudoku-part-ii-9a7019d196a2
#### Code:
Code Reference: https://github.com/tahaemara/real-time-sudoku-solver
#### Youtube:
Taha Emara: https://www.youtube.com/watch?v=Q5F8FteU3OY
