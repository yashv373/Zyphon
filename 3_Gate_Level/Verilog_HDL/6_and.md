module ckt6( 
    input a, 
    input b, 
    output out );
    assign out = a&b; // & operator tells that a has to be and-ed with b and then assigned to out port.
    endmodule