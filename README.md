# Rodwell Graphing Code
Github repo for running and graphing the Rodwell simulation. 

# Instructions 

1. Download the Rodwell Code for Mac and the Sample Rodwell Code Input files, put them in your desktop
2. Open the Rodwell Code and near the top of the code you should see this line: `OPEN(unit=9,FILE="/Users/anabojinov/Desktop/Input_20kW_68deg_10Gal.txt")` change the bolded section so that the file directs to your directory (to find this, you can right click on the file in your finder and click "Get Info," you should then be able to see what name it's under, you might also need to change the input.txt file name to match the name of your input file
3. SAVE the code
4. Open your terminal, you can do this by doing command+space and then searching for "terminal"
5. Now, you can compile and run the code by entering these commands into your terminal, you're basically entering the place where the code is stored, compiling the code, and then running it:
	a. cd Desktop 
	b. gfortran mac_correct_rodwell.f -o a.out -ffree-line-length-512 -ffree-form -Wall
	c. ./a.out

**Other Information**
the output file should pop up in your desktop, it will be in the .dat format 
if you want to run the code again you have to either delete or rename the output file
if you want to exit the compiler simply type "exit" in the terminal
