// File: 1_simple_output.v
// Description: This is the first Verilog circuit in our learning journey.
// It introduces the basic module structure and the concept of assigning a constant value to an output.


module ckt(output y); // a module named ckt is instantiated and inside it we have a declaration of output port y. no inputs, just y.
assign y=1; //this tells that y port  is to be assigned value = 1.
endmodule // closing the module