# Lab 2

## Lincoln Samelson
## Collaborators: Brian Gaydon, Ali Hakimi, Chris Gray
## Principles of Programming: CSCI 3155

####Lab 2: Writeup

_1. Grammars: Synthetic Examples._

A ::= A & A | V

V ::= a | b

**Solutions**
**(a)**

               S1 is in AObjects S2 is in AObjects
            -----------------------------------------
                      S1 & S2 in AObjects
                      
                         S is in VObjects
                     ------------------------
                         S is in AObjects

**(b)**

				Because V => a or b, therefore:
						A => A & A
						A => (A & A) & (A & A)
						A => a & a & a & a
						
				This is ambiguous 
				
				Also:
						A => (A & A) & V
						A => (V & (A & A) & V)
						A => (a & (V & V) & a)
						A => (a & (a & a) & a)
						A => a & a & a & a
						
			    This too is ambiguous
			    
				




