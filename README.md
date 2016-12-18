#**Finding Lane Lines on the Road** 

I used the following sequence of steps to arrive at the solution

1) Grayscale Image 

<img src="https://github.com/shankarananth/CarND-LaneLines-P1/blob/master/debug_images/solidWhiteCurve.jpg1Gray.jpg" width="480" alt="Gray Image" />

2) Guassian Blur 

<img src="https://github.com/shankarananth/CarND-LaneLines-P1/blob/master/debug_images/solidWhiteCurve.jpg2Guass.jpg" width="480" alt="Guass Blur Image" />

3) Canny Edge Detection 

<img src="https://github.com/shankarananth/CarND-LaneLines-P1/blob/master/debug_images/solidWhiteCurve.jpg3Edge.jpg" width="480" alt="Canny Edge Detection Image" />

4) Region of Interest 

<img src="https://github.com/shankarananth/CarND-LaneLines-P1/blob/master/debug_images/solidWhiteCurve.jpg4Mask.jpg" width="480" alt="ROI Image" />

5) Hough Transformation and Extrapolation

<img src="https://github.com/shankarananth/CarND-LaneLines-P1/blob/master/debug_images/solidWhiteCurve.jpg5Hough.jpg" width="480" alt="Hough Image" />

<img src="https://github.com/shankarananth/CarND-LaneLines-P1/blob/master/debug_images/solidWhiteCurve.jpg6Weight.jpg" width="480" alt="Hough Image" />

Some lessons learnt from experience

1) I use Anaconda on windows. Had some difficulty in installing ffmpeg. I used the guideline provided in the following link to solve the issue https://github.com/adaptlearning/adapt_authoring/wiki/Installing-FFmpeg

2) I used a debug folder to save all intermediate image. This helped me a lot in easy tuning of various parameters.

3) I did not attempt the Optional challenge to optimize available time with me. Test runs with current code was not successful.

4) In terms of improvement I could further smooth the lines across frames in video.

5) I did not have experience with Jupyter. It is very different for a coding environment. However after using it I could visibly see the advantage of such an environment.

6) Line Extrapolation - I used y=mx+c to identify extrapolated line (First identify slope with co-ordinates ((y2-y1)/(x2-x1)), Second calculate C and Third idenfy new co-ordiantes based on given y-axis)

Results uploaded to Youtube

Video White
https://youtu.be/D7xby1-8GI0

Video Yellow
https://youtu.be/-qIGKi5mOCA

