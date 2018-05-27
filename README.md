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

# Program in action      


# Result    
