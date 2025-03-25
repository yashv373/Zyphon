// moving forward, lets look at the very first data type in verilog, that is a wire. A wire is very similar to the wire we encounter in real life and if we want internal connections in our verilog circuits that are not explicitly declared ports, we can use wires. remember, that wires are not capable of storage and for that we will encounter a different datatype, namely reg.


module ckt3(input, output);
( input in, output out );
assign out=in;
endmodule

endmodule
