## Real-Time-Sudoku-Solver-OpenCV-and-Keras
Solves a Sudoku puzzle under one second and overlays the solved puzzle on to the original image in real-time. 
This repo consists of Python code for solving sudoku puzzle using Deep Learning and OpenCV in real time(Live Camera).<br>
Main Reference: [Anh Minh Tran](https://www.youtube.com/watch?v=uUtw6Syic6A&list=LLwC_qd6q9vEqDaxU3KdSgPw&index=2&t=236s)

### 🛠 Sample outputs from Custom YOLOv3 model
<img src="https://github.com/snehitvaddi/Real-Time-Sudoku-Solver-OpenCV-and-Keras/blob/master/output/output-gif.gif" width="400">

### 🧬 Algorithim Used
In general Sudoku is solved using Backtracking approch, where it is a bruteforce approch.<br>
Here we are using **Greedy Best First Search approch**!! -> which an optimised version of Naive Back Tracking method ie; Chooses a cell with least number of possibilities to search next.

### 🏃‍♂️ How to Run!!
*Step-1*: Install all required libraries in `requirements.txt` or directly run `pip install -r requirements.txt`<br>
*Step-2*: Directly run all cells of `Sudoku testing.ipynb` file. It does all the imports by itself.<br>
*Step-3*: Nothing else, just get your Sudoku puzzle in front of your camera and solutions will be relayed over their respective positions.<br>
*Step-4*: To stop the camera, click 'Q' on keyboard.

### 📑 Step By Step Explanation:
|    Step      |   What's happening      |   Image      |
|------------------|--------------|-------------------|
|    Step -1 &nbsp;| Reading image from real-time input or a video or an image.|<img src="https://github.com/snehitvaddi/Real-Time-Sudoku-Solver-OpenCV-and-Keras/blob/master/step%20by%20step%20images/1.jpg" width="300"> |
|    Step -2  &nbsp;| Convert input image to black and white. Apply threshold to remove unwanted noice. |<img src="https://github.com/snehitvaddi/Real-Time-Sudoku-Solver-OpenCV-and-Keras/blob/master/step%20by%20step%20images/2.png" width="300"> |
|    Step -3    &nbsp;  | Get boundry of largest contour ie: Outline of sudoku matrix. |<img src="https://github.com/snehitvaddi/Real-Time-Sudoku-Solver-OpenCV-and-Keras/blob/master/step%20by%20step%20images/3.png" width="300"> |
|    Step -4   &nbsp;| In each cell of sudoku matrix, detect if any number is there or not by finding contours. |<img src="ttps://github.com/snehitvaddi/Real-Time-Sudoku-Solver-OpenCV-and-Keras/blob/master/step%20by%20step%20images/5.png" width="300"> |
|    Step -5   &nbsp;| Predict those detected numbers |<img src="https://github.com/snehitvaddi/Real-Time-Sudoku-Solver-OpenCV-and-Keras/blob/master/step%20by%20step%20images/6.png" width="300"> |
|    Step -6  &nbsp;| Input the predicted numbers into  `Sudoku Solving algorithm` and get the out put.| |
|    Step -7  &nbsp;| Overlay the corresponding calculated results on to live image/video.| |

### ✍ Note:
I had trained a custom model for Number prediction. You can use either the existing one or a model of your own.
### 📝 References:
###### Algorithim:<br>
For solving sudoku: https://norvig.com/sudoku.html<br>
Tech With Tim: https://www.youtube.com/watch?v=lK4N8E6uNr4<br>

###### Theoretical:<br>
Sudoku extraction from image: https://medium.com/@neshpatel/solving-sudoku-part-ii-9a7019d196a2 (with python code)<br>
Solving Sudoku Part1: https://medium.com/@neshpatel/solving-sudoku-part-i-7c4bb3097aa7<br>
Solving Sudoku Part2: https://medium.com/@neshpatel/solving-sudoku-part-ii-9a7019d196a2<br>

###### Code:<br>
Code Reference: https://github.com/tahaemara/real-time-sudoku-solver<br>

###### Youtube:<br>
Taha Emara: https://www.youtube.com/watch?v=Q5F8FteU3OY<br>

### 🤝 Lets Connect on [Linkedin](https://www.linkedin.com/in/snehitvaddi/)
