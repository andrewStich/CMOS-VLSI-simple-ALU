# CMOS-VLSI-simple-ALU
CMOS/VLSI design final project. We were asked to design and test a number of CMOS logic gates on the transistor level in order to create a 4-bit ALU that adds, subtracts, and multiplies.

The end-goal of this project was to create an a 4-bit ALU that multiplied, added, and subtracted. It had two 4-bit inputs and a 2-bit select line that would select between the three operations. All transistor-level schematics, test-bench schematics, layouts, and test results can be found in the pdf files.
This project was compiled and ran in cadence-virtuoso 6.

## Addition/Subtraction operation
The addition/subtarction unit was comprised of 4 full adders that were cascaded. It had 5 output bits, the last one being the carry out if addition was selected or the two's compliment identifier if subtraction was selected. These 5 output bits were then sent to the first input of an an 8-bit 2-to-1 mux whose select signal would be low when in addition/subtraction mode.

## Multiplication operation
I deceded to make the multiplication unit combinational. This was an easier device to test, but much more complicated to design as it was comprised of 4 addition/Subtraction units and a multitude of AND and OR gates. It took the two 4-bit inputs and gave an 8-bit output which fed into the second input of the 8-bit mux whose select signal would be high in multiplication mode.

## Group Work and Personal Contribution
Project one was assigned individually while project 2 was assigned to us in groups of 2. I found this project to be especially interesting and fun once I learend how to use the cadence software, so I did most of it in my free time. This led to me doing all the schemetics, testbenches, and layouts and finishing it 3 weeks before it was due. My partner then wrote up the report.
