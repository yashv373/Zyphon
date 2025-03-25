module ckt7( 
    input a, 
    input b, 
    output out );
    assign out=~(a|b); // here again, a | b is same as a 