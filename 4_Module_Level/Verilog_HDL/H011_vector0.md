// Build a circuit that has one 3-bit input, then outputs the same vector, and also splits it into three separate 1-bit outputs. Connect output `o0` to the input vector's position 0, `o1` to position 1, etc.

module ckt11(
input wire [2:0] vec,
output wire [2:0] outv,
output wire o2,
output wire o1,
output wire o0
);
assign outv=vec; // the entire outv vector output is mapped to vec input 
assign o0=vec[0]; // o0 output assign input vector vec's 0th bit position value, and so on.
assign o1=vec[1];
assign o2=vec[2];
endmodule