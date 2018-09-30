# Teqnirvana Assignment

Technical Lib and class details
        
1) ReadStream interface is created and 'line' event is attached for listening.

2) Each new Line is trimmed and forwarded to Merchant function for further processing.

3) In Merchant function line is matched again 4 different Regular Expressions to detect type of line(assignment/query).If line does not match any of the expressions it is declared as undetected type.

4) There are 4 types of lines

 a) Assignment:-assignment lines assign inter-galaxy currency to Roman numeral
 b) Credit:-credit line give currency conversion in units(metal or scrap) with credit value.
 c) HowMuch query:-howmuch query is used to get inter-Galaxy currency value in Arabic decimals.
 d) HowMany query:-howmany query is used to get credit values for inter-Galaxy currency.
 
5) function is used to convert inter-galaxy currency to it's value. Function Works as follows,

a) Convert inter-Galaxy currency array to respective roman numeral,while converting use saved inter-galaxy currency for conversion.
b) Check if constructed roman numeral is valid.
c) Convert that roman numeral to decimal number.


I, II, III, IV, V, VI, VII, VIII, IX, X  (1-10)
X, XX, XXX, XL, L, LX, LXX, LXXX, XC, C. (10-100)
C, CC, CCC, CD, D, DC, DCC, DCCC, CM, M. (100 - 1000)
Reference : https://en.wikipedia.org/wiki/Roman_numerals

