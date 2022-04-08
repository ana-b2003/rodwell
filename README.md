# Rodwell Graphing Code
Github repo for running and graphing the Rodwell simulation. 

# Instructions for mac
1. Download github code to Desktop, also enter the download folder called `rodwell`
	a. You can download by downloading the zip file 
	b. You can also download through the terminal by typing the following command `git clone https://github.com/ana-b2003/rodwell.git`
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

# Graphing output file 
**YOU MUST HAVE PYTHON3 INSTALLED WITH NUMPY, PANDAS, AND MATPLOTLIB** 

1. Open terminal 
2. type the following commands 
3. `cd Desktop/`
4. `cd rodwell/`
5. `python3 nontableReader.py` This will graph the non table data 
6. `python3 tableReader.py`  This will graph all the table data

## nontableReader code legend 
  0 - hours  
  1 - TOTAL ENERGY INPUT BTU  
  2 - SEASONAL ENERGY INPUT BTU  
  3 - SEASONAL ENERGY INPUT GAL FUEL  
  4 - SEASONAL ENERGY RATE BTU/HR  
  5 - TOTAL ENERGY INPUT GAL FUEL  
  6 - AVERAGE LB. WATER PER LB. FUEL  
  7 - SEASONAL LB. WATER PER LB. FUEL  
  8 - ENERGY FROM AIR TO ICE BTU  
  9 - SEASONAL ENERGY LOSS, AIR TO ICE BTU  
  10 - TOTAL WATER WITHDRAWN GAL  
  11 - SEASONAL WATER WITHDRAWN GAL  
  12 - TOTAL WATER LOSS GAL  
  13 - SEASONAL WATER LOSS GAL  
