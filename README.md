# cmyk_stitch
Print Oriented Processing Sketch.

## What is this?
I wrote this sketch for my FRESH portfolio showcase. It takes CMYK color channels and processes them into a series of lines.
These lines when layered in a print will create an approximation of the original image, however with a unique texture as a result of the code. 


## How to

### file prep
***Photoshop*** 
1. Open Desired Image File
2. If Image is in RGB go to -> *Image* -> *Mode* -> *CMYK Color*
3. Navigate to the *Channels* Panel
4. Select the *Cyan* channel right click and select *Duplicate Channel* 
5. In the window that opens go to the *destination* section and select the *document* dropdown
6. In the *document* dropdown select *new*
7. Name the file what you want, I would suggest that you name it something line *name*_cyan
8. Select *Ok* 
9. Navigate to the new document
10. Go to  ->*Image* -> *Mode* -> *RGB Color*
11. Save the file out as a Jpeg to the *data* folder included with the code
12. Repeat steps 4-11 for the Magenta, Yellow, and Key Channels.

*Note:*I would recommend bright images for this process, dark ones can get very muddles in the printing process. Image size can also present problems, I would recommend using images that arent too large. 

### Prepping and running the code
***Processing Sketch***
13. Open the processing Sketch
14. In the *setup* section set it to the size to the same as the images (ensures that everything saves correctly).
15. Place the filenames for the CMYK channels in the corresponding sections of the code
    ex: `cyan = loadImage("yourcyanchannel.jpg");`
 16. At the top of the code there are *cellsize* variables for the individual channels. Set them to your desired size 
 *Note:* Ive found that a cellsize of 10 usually produces the best results.
 17. Press Run. It may take a moment depending on the image sizes. 
 
 ### Accessing the Processed Images and Prepping them for Print
 ***File Manager***
 18. Acess the Folder that Contains the .pde file
 19. In that folder will be the images labeled as cyan_0001, magenta_0002, yellow_0003 and key__0004.
 20. Select them all and open in Photoshop
 ***Photoshop***
 21. In whichever image you access first go to *image* -> *mode* -> *grayscale*
 22. Save the file out as a jpeg to a secondary folder, this will prevent overwriting if you run the code again. 
 23. Repeat steps 4 & 5 for the rest of the output images
 *Note:* from here there are a variety of different ways you can get this prepped for print. I'm going to be showing you how I do it most of the time. 
 ***InDesign***
 24. Create a document that is your ideal print size (usually 8.5x11 or 9x12 for me)
 25.prest cmd+d to place the cyan layer in
 26. Size it to your print / margin area
 28. Select the Image within the frame
 29. Go to *fx*->*transparency*->*multiply
 30. Set the image color to cyan from the color panel
 31. Duplicate the image, and delete the image from the frame. 
 32. Duplicate the frame so that there are 3. Layer them all on top of each other. 
 33. Hide the top two frames in the layer panel.
 34. Repeat Steps 25-30 With the Magenta, Yellow, and Key Layers. Revealing each frame int the panel after every time. 
 35. Print 
 
 ### In Closing
 This is can be quite a process. If processing had better ways of contending with CMYK images this would be a lot more automated. As of now this is the best way I've found to do this. 
 
 Thank you for checking this out!
 
 Max Ettel
 Sept 18th 2019.
 




