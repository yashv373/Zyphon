//Create a module with 3 inputs and 4 outputs that behaves like wires that makes these connections:
//a -> w
//b -> x
//b -> y
//c -> z

module ckt4( 
    input a,b,c,
    output w,x,y,z ); // declaring a module named ckt4, with 3 inputs a,b and c; and 4 outputs w,x,y,z
    assign w=a; //a -> w
    assign x=b; //b -> x
    assign y=b; // b-> y
    assign z=c; //c -> z
endmodule // end the module.