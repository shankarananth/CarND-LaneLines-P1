#**Finding Lane Lines on the Road** 

I used the following sequence of steps to arrive at the solution
1) Grayscale Image 
2) Guassian Blur 
3) Canny Edge Detection 
4) Region of Interest 
5) Hough Transformation

Some lessons learnt from experience

1) I use Anaconda on windows. Had some difficulty in installing ffmpeg. I used the guideline provided in the following link to solve the issue https://github.com/adaptlearning/adapt_authoring/wiki/Installing-FFmpeg

2) I used a debug folder to save all intermediate image. This helped me a lot in easy tuning of various parameters.

3) I did not attempt the Optional challenge to optimize available time with me. Test runs with current code was not successful.

4) In terms of improvement I could further smooth the lines across frames in video.

5) I did not have experience with Jupyter. It is very different for a coding environment. However after using it I could visibly see the advantage of such an environment.

Results uploaded to Youtube

Video White
[![Video White](https://github.com/CYHSM/carnd/blob/master/CarND-LaneLines-P1/white.gif?raw=true)](https://youtu.be/D7xby1-8GI0) Video Yellow
[![Video Yellow](https://github.com/CYHSM/carnd/blob/master/CarND-LaneLines-P1/yellow.gif?raw=true)](https://youtu.be/-qIGKi5mOCA)

