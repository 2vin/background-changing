# background-changing
Modifying OpenCV's grabcut implementation to change background

This program can be used to change the background of an image by applying grabcut algorithm.   

# Compile    
g++ background-change.cpp -o main \`pkg-config --cflags --libs opencv\`    

# Usage    
./main fg_image bg_image    
(where, fg_image is the foreground image, and bg_image is the background image)    

This will open the image in a window where you can select foreground and background pixels.    
In order to select background pixels, press 'Ctrl' and click+move over the background region. Similarly, in order to select foreground pixels, press 'Shift' and click+move over the foreground region. Once the selection process is completed, press 'n' to perform grabcut.     
(Note: Pressing 'n' multiple times will refine the resulting mask)

# Example    
./main ./data/in1.jpg ./data/in2.jpg    

# Program in action      
![Alt text](https://user-images.githubusercontent.com/38634222/40589609-a5f2b922-620d-11e8-9d16-92102a0d2b65.gif)

# Result    
Input images:    
<a href="Input1"><img src="https://raw.githubusercontent.com/2vin/background-changing/master/data/in1.jpg" align="left" height="208" width="313" ></a>
<a href="Input2"><img src="https://raw.githubusercontent.com/2vin/background-changing/master/data/in2.jpg" align="right" height="208" width="313" ></a>     

Result Image:    
<a href="Result"><img src="https://raw.githubusercontent.com/2vin/background-changing/master/data/Result.jpg" align="right" height="208" width="313" ></a>
