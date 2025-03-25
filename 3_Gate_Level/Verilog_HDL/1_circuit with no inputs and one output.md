//we will begin learning verilog using practical methodology.
//all of the codes here on out will be heavily commented to explain the process and logic.
//we will begin from the basics and move upto complex circuits
//for a structure bottom-up approach, we're following the list by HDLbits.
//The first task is to describe a verilog circuit with no inputs and 1 output. we need to make sure output port always gives output as 1 or logic high.

module ckt(output y); // a module named ckt is instantiated and inside it we have a declaration of output port y. no inputs, just y.
assign y=1; //this tells that y port  is to be assigned value = 1.
endmodule // closing the module