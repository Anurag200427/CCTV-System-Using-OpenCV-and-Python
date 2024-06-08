# CCTV-System-Using-OpenCV-and-Python
This is just a minor project in which we are using simple python tools like openCV to make a functional CCTV system and face detection.
First up when the program runs we create a file by name of recordings.mp4v when the video will be stored.
def main():
    cap = cv2.VideoCapture(0)

    first_frame = None
    
    fourcc = cv2.VideoWriter_fourcc(*'MJPG')
    out = cv2.VideoWriter('Recording.mp4v', fourcc, 20.0, (640, 480))
     
    while True:
        ret, frame = cap.read()
        if not ret:
            break
a video device is selected and the frames are being read. If the source cant be read then the loop breaks.
We create 3 window for cctv , grey and thresh.
"q" is the key to end the program and break the loop.
