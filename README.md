## Real-Time-Sudoku-Solver-OpenCV-and-Keras
Python application to solve Sudoku puzzle and overlays solution on to real image in real-time. 

This project is solely inspired from **AnhMinhTran's** [Youtube Video](https://www.youtube.com/watch?v=uUtw6Syic6A&list=LLwC_qd6q9vEqDaxU3KdSgPw&index=2&t=236s).

### 🛠 Sample output
<img src="https://github.com/snehitvaddi/Real-Time-Sudoku-Solver-OpenCV-and-Keras/blob/master/output/output-gif.gif" width="400">

### 🧠 Algorithim Used
In general Sudoku is solved using Backtracking approch, which is a bruteforce approch.<br>
Here we are using **Greedy Best First Search approch** (An optimised version of Naive Back Tracking method) ie; Chooses a cell with least number of possibilities to search next.

### 🏃‍♂️ How to Run!!
*Step-1*: Install all required libraries in `requirements.txt` or directly run `pip install -r requirements.txt`<br>
*Step-2*: Directly run all cells of `Sudoku testing.ipynb` file. It does all the imports by itself.<br>
*Step-3*: Nothing else, just get your Sudoku puzzle in front of your camera and solutions will be relayed over their respective positions.<br>
*Step-4*: To stop the camera, click 'Q' on keyboard.

### 📑 Step By Step Explanation
|   What's happening      |   Image      |
|--------------|-------------------|
| Step-1: Reading image from real-time input or a video or an image.|<img src="https://github.com/snehitvaddi/Real-Time-Sudoku-Solver-OpenCV-and-Keras/blob/master/step%20by%20step%20images/1.jpg" width="200"> |
|    Step-2: Convert input image to black and white. Apply threshold to remove unwanted noice. |<img src="https://github.com/snehitvaddi/Real-Time-Sudoku-Solver-OpenCV-and-Keras/blob/master/step%20by%20step%20images/2.png" width="200"> |
|    Step-3: Get boundry of largest contour ie: Outline of sudoku matrix. |<img src="https://github.com/snehitvaddi/Real-Time-Sudoku-Solver-OpenCV-and-Keras/blob/master/step%20by%20step%20images/3.png" width="200"> |
|    Step-4: In each cell of sudoku matrix, detect if any number is there or not by finding contours. |<img src="ttps://github.com/snehitvaddi/Real-Time-Sudoku-Solver-OpenCV-and-Keras/blob/master/step%20by%20step%20images/5.png" width="200"> |
|    Step-5: Predict those detected numbers |<img src="https://github.com/snehitvaddi/Real-Time-Sudoku-Solver-OpenCV-and-Keras/blob/master/step%20by%20step%20images/6.png" width="300"> |
|    Step-6: Input the predicted numbers into  `Sudoku Solving algorithm` and get the out put.| |
|    Step-7: Overlay the corresponding calculated results on to live image/video.| <img src="https://github.com/snehitvaddi/Real-Time-Sudoku-Solver-OpenCV-and-Keras/blob/master/output/output-gif.gif" width="200">|

### ✍ Note
I had trained a custom model for Number prediction. You can use either the existing one or a model of your own.
### 📝 References
###### Algorithim:<br>
For solving sudoku: https://norvig.com/sudoku.html<br>
Tech With Tim: https://www.youtube.com/watch?v=lK4N8E6uNr4<br>

###### Theoretical:<br>
Sudoku extraction from image: https://medium.com/@neshpatel/solving-sudoku-part-ii-9a7019d196a2 (with python code)<br>
Solving Sudoku Part1: https://medium.com/@neshpatel/solving-sudoku-part-i-7c4bb3097aa7<br>
Solving Sudoku Part2: https://medium.com/@neshpatel/solving-sudoku-part-ii-9a7019d196a2<br>

###### Code:<br>
**Code Reference:** 
* https://github.com/tahaemara/real-time-sudoku-solver
* **https://aakashjhawar.medium.com/sudoku-solver-using-opencv-and-dl-part-2-bbe0e6ac87c5**<br>

###### Youtube:<br>
Taha Emara: https://www.youtube.com/watch?v=Q5F8FteU3OY<br>

### Connect with Author
🤝 LinkedIn: [Lets Connect](https://www.linkedin.com/in/snehitvaddi/)<br>
