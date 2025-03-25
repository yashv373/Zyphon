module ckt7( 
    input a, 
    input b, 
    output out );
    assign out=~(a|b); // here again, a | b is same as a OR-ed with b. since we need a nor gate, this entire thing is the negated using '~' operator and then assigned to the out terminal.
endm