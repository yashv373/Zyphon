// Build a combinational circuit with four inputs, in[3:0].
// There are 3 outputs:
// - out_and: output of a 4-input AND gate.
// - out_or: output of a 4-input OR gate.
// - out_xor: output of a 4-input XOR gate.

module ckt15(input [3:0] in, output out_or, out_and, out_xor);
assign out_and=&in;
a