# AI Virtual Mouse with Motion Games "Motion is All You Need". Our Product uses state-of-the-art motion capture technology to enable users to play games in radically new ways using machine learning.

# Customizable Product

We haved shipped three games and all are customizable and happy to say that our product will instantly train the gestures in all the games that is hand, face and body gestures. What was happening in the past that people are making the prouct but that are pre-trained [ means that are not customizable ] but our product have proved that customization is possible.

# Inspiration
Gaming is often associated with sitting for long periods of time in front of a computer screen, which can have negative physical effects. In recent years, consoles such as the Kinect and Wii have been created to encourage physical fitness through games such as "Just Dance". However, these consoles are simply incompatible with many of the computer and arcade games that we love and cherish.

# What it does

We came up with AI Rodent Playtime at Rajasthan IT Day Hackathon wanting to create a technological solution that pushes the boundaries of what we’re used to and what we can expect. Our product delivers on that by introducing a new, cost-efficient, and platform-agnostic solution to universally interact with video games through motion capture, and reimagining the gaming experience.

Using state-of-the-art machine learning models, AI Rodent Playtime can detect over 500 features on the human body (468 facial features, 21 hand features, and 33 body features) and use these features as control inputs to any video game. AI Rodent Playtime operates in 3 modes: using hand gestures, face gestures, or full-body gestures. We ship certain games out-of-the-box such as Flappy Bird and Snake, with predefined gesture-to-key mappings, so you can play the game directly with the click of a button. For many of these games, jumping in real-life (body gesture) /opening the mouth (face gesture) will be mapped to pressing the "space-bar"/"up" button.

However, the true power of our product comes with customization. Every simple possible pose can be trained and clustered to provide a custom command. Our Product will also play a role in creating a more inclusive gaming space for people with accessibility needs, who might not physically be able to operate a keyboard dexterously.


# How we built it 
First, a camera feed is taken through Python OpenCV. We then use Google's Mediapipe models to estimate the positions of the features of our subject. To learn a new gesture, we first take a capture of the gesture and store its feature coordinates generated by Mediapipe. Then, for future poses, we compute a similarity score using euclidean distances. If this score is below a certain threshold, we conclude that this gesture is the one we trained on. An annotated image is generated as an output through OpenCV. The actual keyboard presses are done using PyAutoGUI.

We used Tkinter and custom Tkinter to create a graphical user interface (GUI) where users can switch between different gesture modes, as well as select from our current offering of games. We used MongoDB as our database to keep track of scores and make a universal leaderboard.

# Challenges we ran into

Our team didn't have much experience with combined python and ml stack before, so it was a big learning curve. Two of us didn't have a lot of experience in Python. We ran into many dependencies issues, and package import errors, which took a lot of time to resolve. When we initially were trying to set up MongoDB, we also kept timing out for weird reasons. But the biggest challenge was probably trying to write code while running on 6 hours of sleep...

# Accomplishments that we're proud of
We are very proud to have been able to execute our original idea from start to finish. We managed to actually play games through motion capture, both with our faces, our bodies, and our hands. We were able to store new gestures, and these gestures were detected with very high precision and low recall after careful hyperparameter tuning.

# What we learned
We learned a lot, both from a technical and non-technical perspective. From a technical perspective, we learned a lot about the tech stack (Python + MongoDB + working with Machine Learning models). From a non-technical perspective, we worked a lot working together as a team and divided up tasks!

# What's next for our Product
We would like to implement a better GUI for our application and release it for a small subscription fee as we believe there is a market for people that would be willing to invest money into an application that will help them automate and speed up everyday tasks while providing the ability to play any game they want the way they would like. Furthermore, this could be an interesting niche market to help gamify muscle rehabilition, especially for children.

# Built With
- Json
- MediaPipe
- Mongo-DB
- Open-CV
- PY-GAME
- PY-SIMPLEGUI
- PYTHON
- TKINTER

# Libraries you need to install if you want to run our product 
- cv2
- mediapipe
- numpy
- pyautogui
- autopy
- customtkinter
- os
- tkinter
- PIL
- random
- json
- bcrypt

# Snap-Shot of AI Mouse and Motion Game

## Home page:
![hand](./assets/git%20readme/Home.jpeg)

## Snap-Shot of AI Mouse :-

### Hand Gesture detected:
![hand](./assets/git%20readme/hand%20gesture.jpeg)

### Left Click:
![left](./assets/git%20readme/left%20click.jpeg)

### Right Click:
![left](./assets/git%20readme/right%20click.jpeg)

### Double Click:
![left](./assets/git%20readme/double%20click.jpeg)

### Scroll-up:
![recent](./assets/git%20readme/scroll-up.jpeg)

### Scroll-down:
![recent](./assets/git%20readme/scroll-down.jpeg)

### and other features are there in the video.


## Snap-Shot of AI Motion Game :-

### Snake Game:
![hand](./assets/git%20readme/snake.jpeg)

### Flappy bird Game:
![left](./assets/git%20readme/flappy-bird.jpeg)

### Tetris Game:
![left](./assets/git%20readme/Ttris.jpeg)

### and other features are there in the video.


---
# Demo video [Link](https://www.youtube.com/watch?v=Jr0UayRC6I8)
