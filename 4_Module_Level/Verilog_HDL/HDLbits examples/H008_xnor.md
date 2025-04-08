module ckt7( 
    input a, 
    input b, 
    output out );
    assign out=~(a^b); // same as example 7 , we use the ^ operator to do a XOR-ed with b and the negate to get XNOR-ed output.
endmodule