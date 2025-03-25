module ckt7( 
    input a, 
    input b, 
    output out );
    assign out=~(a^b); // same 
endmodule