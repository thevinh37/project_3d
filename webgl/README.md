TA: Garett Ridge

All the extera credits was done for this project.

Instruction:

	r   start and stop the rotation both cubes.

	i   move the camera nearer along the z-axis

	o 	move the camera farther away along the z-axis

	t   start and stop the rotation of the texture map itself on all faces of cube #1 around the center 
		of each face at a rate of 15 rpm

	s 	start and stop the continuous scrolling the texture map on cube #2. Translate the texture 
		varying the s texture coordinate only by 1 unit per second.

This project i impelemented two cubes with texture. both cube have dimensions 2x2x2. texture for cube
one is set to nearest neighbor by stting gl.TEXTURE_MAG_FILTER and gl.TEXTURE_MIN_FILTER both to 
gl.NEAREST. which means that WebGL will uses a filter that determines the colour of a given point just
by looking for the nearest point in the original image.
texture for cube 2 is set to tri-linear filtering with Mipmaps by setting gl.TEXTURE_MAG_FILTER to gl.LINEAR and 
gl.TEXTURE_MIN_FILTER to gl.LINEAR_MIPMAP_NEAREST. FOV is set to 50 degrees and cube one in at (-4,0,0) and cube 2 is 
at (-4,0,0). using three uniform matiries(uMVMatrix, uPMatrix,uTMatrix) i was able to translate and rotate around the 
cubes and scroll and rotate texture on face of each cube. the speed of rotatin was calulated using time 
and mapping the value to radian using degree to raidan function and all the speed calculated and 
verifyed.

this project was done using gl-matrix on google chrome Version 56.0.2924.87 (64-bit) and webgl 1. the 
key values in the code uses chrome key value mapping and might not work with other browsers.


all the extera credits were done and applyed and can be seen by running and using s ant t key. (check the Instruction)

sources:
http://learningwebgl.com/
gl-matrix library
opengl official website






