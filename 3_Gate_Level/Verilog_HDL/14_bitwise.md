//Build a circuit that has two 3-bit inputs that computes the bitwise-OR of the two vectors, the logical-OR of the two vectors, and the inverse (NOT) of both vectors. Place the inverse of `b` in the upper half of `out_not` (i.e., bits [5:3]), and the inverse of `a` in the lower half.

module ckt14 (
input [2:0] a,
    input [2:0] b,
    output [2:0] out_or_bitwise,
    output out_or_logical,
    output [5:0] out_not
);
  assign out_or_bitwise = a | b;      // Bitwise OR
  assign out_or_logical = |(a || b);  // Logical OR (reduced to 1 bit)
  assign out_not = {~b, ~a};          // Concatenated NOT of 'b' (upper) and 'a' (lower)

endmodule