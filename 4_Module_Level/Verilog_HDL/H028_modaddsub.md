module top_module(
    input [31:0] a,
    input [31:0] b,
    input sub,
    output [31:0] sum
);
add16 a1(a[15:0],b[15:0]);
add16 a2();
endmodule
