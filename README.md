# RSC Overview

* RSC stands for "Relatively Simple Computer"
* It consists of several digitally created registers and PLD circuits.

# How does it work?

* The RSC works by connecting the created registers to one another and a control register that determines when certain values will need to be passed.
* In order for the RSC to perform an operation, it needs bytecode to be inserted. To do this, we create an assembly program that performs the requested operation, convert it to bytecode using an RSC Emulator. Save the bytecode in a text file, and then load said text file into the RSC and tick the clock.

# How do I set it up?

1) In order to open this file, you will need to download [Logism](https://sourceforge.net/projects/circuit/).
2) Once installed, download the zip file for this repository, and extract the files.
*   The folder will contain the RSC, custom_reg, PLDs circuits as well as ram1, ram2 and ram3 text files
3) Open Logism, click "File", and open the RSC file.
*   If asked to select the "custom_reg" file upon opening the RSC file, select the "custom_reg" file you downloaded
4) The text files you've extracted are assembly code that perform different functions.
5) If you wish to load a text file into the RSC, you must download an RSC Emulator. 
6) Once downloaded, paste the code from the file into the emulator and click "compile." Use CRT-A to select the outputted bytecode and CRT-C to copy it.
7) Create a text file and copy "v2.0 raw" as the first line of the file, move to the next line, and paste the copied byte code, and save.
8) Go to the RSC and click on the operation module and select "Load Image"
9) Select the saved text file with the bytecode and then tick the clock until its computation is complete.
10) You've just ran your first program in this RSC! To run more operations, create assembly code to perform and then follow the byte code convertion instructions. Good Luck!

*Note: Under under the simulate tab, select your ticking frequency as 32 Hertz and click "enable ticks." This will let the program do the clock ticking faster making it easier for you to know when its computation is completed.*
