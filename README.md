Download Link: https://assignmentchef.com/product/solved-cse_ece-478-assignment-1-no-time-to-die
<br>
In the yet-to-be-released movie, <em>No Time to Die</em>, 007 has to trace the evil of Ernst Stavro Blofield, a.k.a. Franz Oberhauser, his nemesis from <em>Spectre</em>. 007 and Dr. Swann start from London, M’s office, but they are being followed by S.P.E.C.T.R.E.’s thugs.

<strong>Q </strong>advises you to cover your tracks by generating fake images. To teach you, <em>007</em>, <strong>Q </strong>has shown you an example of image matting(chroma-keying) where you will take an image of yourself on a green screen and add a fake background to it. How does the green screen help in this task?

(a) foreground image                     (b) background image                                  (c) result

<ol>

 <li>Generate images for your fake trail to leave for Blofield using this method.

  <ul>

   <li>Test your implementation using the provided foreground(jpg) and background(bg.jpg).</li>

   <li>Graft <em>007 </em>(jpg) onto Bond’s Skyfall mansion. Find this mansion’s image from the internet.</li>

   <li>Be creative and do the same procedure with a background image of your choice with you in it! You can take any foreground green-screen image from the internet.</li>

  </ul></li>

 <li>As you are a focused agent, you are also worried about how many images you can store on the <em>MI6 </em>cloud with a size of 4 GB. If your fake trail colour images happen to have a size of 1280 x 720, and are stored for displaying on standard displays, calculate the number of images you can store in the cloud.</li>

</ol>

<em>This will tell you how far you can escape, 007. Trust no one, James….</em>

Figure 2: <em>007 </em>and Dr. Swann in his <em>Aston Martin DB5</em>

This is a covert operation. Report to M about why you are doing any step theoretically along with your results. Do not share details of the mission with anyone else.

2.  <strong>MI6 Storage Issues : Part 1</strong>

Figure 3: <strong>M</strong>’s command center at MI6

In the movie, <em>Skyfall</em>, Silva hacked <strong>M</strong>’s computer to obtain info on the field agents to compromise <em>MI6 </em>and its digital network. Now <strong>Q </strong>has to work on a non-compromised system with very little storage. <strong>Q </strong>has retrieved image data on Silva, unfortunately they are very large for the system to handle.

Before you go on your assignment, <strong>M </strong>wants you to debrief your knowledge on image sizes. Calculate the dimensions of a square colour image that is used for <em>MI6 </em>command center displays. The image occupies a size of 168.75 MB.

<h3>3.  Don’t fly too close to the sun</h3>

The subminiature camera is an ultra-compact and portable still camera, primarily used for espionage and surveillance purposes. The <em>MI6 </em>utilized such devices, manufactured by their research and development division. They first appeared in the 1969 James Bond film, On Her Majesty’s Secret Service.

<h2>Figure 4: <em>007 </em>taking a photo of the target</h2>

You have been assigned the mission of taking the photo of some very small enemy insignia, which is heavily guarded. You have to take the picture from as far away as possible, to avoid being shot.

The height of the insignia is t = 32.8cm, and your camera has a square CCD sensor of dimensions 10 x 10 mm with 1024 x 1024 pixels. Focal length the camera lens is adjusted to 62.5cm. You need to ensure that the insignia covers atleast 50 pixels in height, in your captured image, to be readable. What is the farthest distance d you can be from the insignia? Report d to the nearest integer.

<ol start="4">

 <li><strong>Le Chiffre Strikes Again!</strong></li>

</ol>

In the movie, <em>Casino Royale</em>, Le Chiffre sends out a list of targets from MI6 to exterminate. The targets have been sent out such that the original image was corrupted by some procedure. Fortunately <em>007 </em>intercepts those images in Montenegro to alert MI6 after a field agent was taken out. MI6 has the correct images of all targets and Bond knows the corruption procedure is same.

Use your DIP skills from lecture 2 to assist <em>007</em>.

<ol>

 <li>Write a function bitQuantizeImage which takes an 8-bit image im and k, the number of bits to which the image needs to be quantized to and returns the k-bit quantized image. (10 points)</li>

 <li><strong>M </strong>wants an experienced hand to take this assignment, so prove yourself by running the above function on <em>007 </em>jpg and find all possible quantization results (k=1 to k=8).</li>

 <li><strong>M </strong>is still not satisfied enough, so she commands you to show all the bit planes of <em>007 </em>jpg. Pass the test.</li>

</ol>

(a) <em>007 </em>test1.jpg                                                                      (b) <em>007 </em>test2.jpg

<ol start="4">

 <li>Now that you have passed, you are declared fit for active duty. Help <em>007 </em>guess the corruption procedure for a target <em>person</em>’s image, <em>person </em>jpg, using the above functions. The correct images that you know for that corresponding <em>person </em>from the database is represented by <em>person</em>.jpg</li>

</ol>

You will be selecting the target person for whom you will be guessing the corruption procedure using the following method out of the following names {Q, M, Mallory, Tanner, Moneypenny}.

Calculate the modulus of your roll number against 5. Say it is k.

<ul>

 <li>For k = 0 select <strong>Q </strong>(corresponding files are jpg and q corrupt.jpg)</li>

 <li>For k = 1 select Moneypenny (corresponding files are jpg and moneypenny corrupt.jpg)</li>

 <li>For k = 2 select Mallory (corresponding files are jpg and mallory corrupt.jpg)</li>

 <li>For k = 3 select <strong>M </strong>(corresponding files are jpg and m corrupt.jpg)</li>

 <li>For k = 4 select Tanner (corresponding files are jpg and tanner corrupt.jpg)</li>

</ul>

(a) m.jpg                                                                             (b) m corrupt.jpg

(a) mallory.jpg                                                                 (b) mallory corrupt.jpg

(a) q.jpg                                                                              (b) q corrupt.jpg

(a) tanner.jpg                                                                   (b) tanner corrupt.jpg

Good luck on the assignment, <em>007</em>. As always, <strong>M </strong>expects reasons for all the tests and your assignment, so do include that.

<ol start="5">

 <li>(20 points) <em>007 </em><strong>and Quantum.</strong></li>

</ol>

<h2>Figure 10: The low light photograph</h2>

In the movie <em>Quantum of Solace</em>, <em>007 </em>follows Dominic Greene to Breganz, Austria. He infiltrates the secret meeting and sees the members of the Organization Quantum. However the picture is taken in very low light and saved as quantum bad.jpg.

As <strong>Q </strong>you have the following tasks,

<ol>

 <li>Write a function linContrastStretching which takes any image im, integers a and b that enhances the contrast such that the resulting intensity range is [<em>a,b</em>] .</li>

 <li>Use this function to improve the intensity of the quantum bad.jpg and assist <em>007</em>.</li>

</ol>

<strong>M </strong>wants you to debrief on your work in Breganz and has all your passports and credit cards on hold until then. Explain the improvement the contrast theoretically, so that she releases your documents and you can go on the next assignment with <em>007</em>.

<ol start="6">

 <li>(50 points) <strong>Think about your sins</strong>!</li>

</ol>

In the movie, <em>007 </em>finds talks to Mr.White about how to find Oberhauser, the S.P.E.C.T.R.E. mastermind. Mr. White tells him to go to Dr. Madeleine Swann, his daughter. Turns out, Madeleine has only an image file named Map.jpg. <em>007 </em>must use his Digital Image Processing skills to retrieve information.

<strong>M </strong>expects you to plot the histograms of images before and after you apply some histogram processing function. Since this is a covert operation, you will <strong>NOT </strong>be using any inbuilt functions for implementing the histogram processing operations. Perform the following operations:

<ol>

 <li>Write a function histEqualization which takes a grayscale image im, and applies histogram equalization on the entire image.</li>

 <li>Write a function histMatching which takes an input image and a reference image and applies histogram Matching on the input image by matching the histogram with that of the reference image.</li>

 <li>You are supposed to document the mathematical formulae for the function used above. Write them after implementation using markdown math/latex.(Refer Tutorial 1)</li>

 <li><strong>Q </strong>asks you to practice histEqualization on practice range1.jpg and jpg.</li>

</ol>

(a) practice range1.jpg                                                                     (b) hist.jpg

<em>007 </em>now contacts Dr. Madeleine to find Oberhauser. He finds a weird image by the name Map.jpg. Immediately <em>007 </em>realises that this is a map of a known place and pulls up a satellite image of the Sahara Desert by the name satellite img.jpg.

(a) Map.jpg                                                                      (b) satellite image.jpg

Decipher the map using the satellite image by applying histMatching. Somewhere in the map there will be an indicative piece of string denoting the name of a person who died. Also, for another task, <strong>remember </strong>the name of this person.

Figure 13: <em>007 </em>and Dr. Swann at Blofield’s place, Sahara

<h3>7. (30 points) The villains of 007</h3>

An integral part of every <em>007 </em>movie are Bond’s supervillains.

<em>Your weakest links are your emotions, James. They make you predictable and unfortunately, vulnerable.</em>

<ol>

 <li>Write a function piecewiseLinTransform to implement a piecewise linear transform</li>

</ol>

(1)

The function takes an input grayscale image, coefficients <em>K</em><sub>1</sub>,<em>K</em><sub>2 </sub>and intervals [<em>a,b</em>] for each linear segment and produces the transformed output image.

<ol start="2">

 <li>Run the images through piecewiseLinTransform on jpg and bondvillain2.jpg. The piecewise linear functions to be used are given for each image.</li>

 <li>Take any image of any from the internet and run piecewiseLinTransform using any custom piecewise linear function that you like. Plot the function used.</li>

</ol>

Also, the psychiatrist on duty asks you to check your awareness, ’Do you notice any difference in the piecewise linear transforms of the two images, especially in the text overlay?’ Answer him with valid reasoning.

<h3>8. (30 points) Tomorrow Never Dies</h3>

In the 1997 movie, <em>Tomorrow Never Dies 007 </em>is tracking Elliot Carver’s stealth boat that will fire two missiles at H.M.S. Bedford of the British fleet. However it is very dark out in the South China Sea.

Step up into the role of <em>007 </em>and use gamma transform to capture Elliot Carver. <strong>Convert the images to grayscale </strong>before applying any transform.

<ol>

 <li>Write a function gammaTransform that implements <em>s </em>= <em>r<sup>γ </sup></em>on a <strong>grayscale </strong>image and vary <em>γ</em>.</li>

 <li>Use this function on png and increase illumination in the image. Report value of gamma used.</li>

 <li>Use this function on png and hide yourself as you try to apprehend Carver. Make illumination lesser. Report value of gamma used.</li>

 <li>Use this function on your Aston Martin DBS image, aston invisible.jpg to see the numberplate <strong>clearly </strong>so that you can travel to London to report for duty. You will be evaluated on how clear the number plate is after the transformation.</li>

</ol>

<h2>Figure 16: stealth.png</h2>

<h2>Figure 17: aston invisible.jpg</h2>

<ol start="9">

 <li>(40 points) <strong>Is that the best you got?</strong></li>

</ol>

Use the name of the person you found from <strong>Q6 </strong>to access the images needed for this task.

Use this link by putting the name with all lowercase letters:

https://tinyurl.com/&lt;name of person&gt;-dead

<ol>

 <li>You will find 4 grayscale images (jpg, james2.jpg, james3.jpg, james4.jpg) with different contrast levels, which correspond to parts of the same image.</li>

 <li>Retrieve the original image using these four images as best you can. You can use any combinations of techniques used in this assignment.</li>

 <li>You will be evaluated on how uniform your final output looks.</li>

</ol>

<h2>Figure 18: <em>Fin</em></h2>