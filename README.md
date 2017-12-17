# Slurpys

Slurpys

Description

Recognizing strings based on a set of restrictions is a common computational problem. 
A Slurpy is a string of characters that has certain properties. Your program will read in strings of characters and output whether or not they are Slurpys. 

A Slump is a character string that has the following properties: 

1. Its first character is either a 'D' or an 'E'. 

2. The first character is followed by a string of one or more 'F's. 

3. The string of one or more 'F's is followed by either a Slump or a 'G'. The Slump or 'G' that follows the F's ends the Slump. For example DFFEFFFG is a Slump since it has a 'D' for its first character, followed by a string of two F's, and ended by the Slump 'EFFFG'. 

4. Nothing else is a Slump. 

A Slimp is a character string that has the following properties: 

1. Its first character is an 'A'. 

2. If it is a two character Slimp then its second and last character is an 'H'. 

3. If it is not a two character Slimp then it is in one of these two forms: 
a) 'A' followed by 'B' followed by a Slimp followed by a 'C'. 
b) 'A' followed by a Slump (see above) followed by a 'C'. 

4. Nothing else is a Slimp. 

A Slurpy is a character string that consists of a Slimp followed by a Slump. 

Examples 

Slumps:        DFG, EFG, DFFFFFG, DFDFDFDFG, DFEFFFFFG

Not Slumps:    DFEFF, EFAHG, DEFG, DG, EFFFFDG

Slimps:        AH, ABAHC, ABABAHCC, ADFGC, ADFFFFGC, ABAEFGCC, ADFDFGC

Not Slimps:    ABC, ABAH, DFGC, ABABAHC, SLIMP, ADGC

Slurpys:       AHDFG, ADFGCDFFFFFG, ABAEFGCCDFEFFFFFG

Not Slurpys:   AHDFGA, DFGAH, ABABCC
Input

The first line contains an integer N between 1 and 10 describing how many strings of characters are represented. The next N lines each contain a string of 1 to 60 alpha characters.

Output

The first line of output should read SLURPYS OUTPUT. Each of the next N lines of output should consist of either YES or NO depending on whether or not the corresponding input line is a Slurpy. The last line of output should read END OF OUTPUT.

Sample Input

2
AHDFG
DFGAH

Sample Output

SLURPYS OUTPUT
YES
NO
END OF OUTPUT
