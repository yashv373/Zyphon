module top_module(
    input [31:0] a,
    input [31:0] b,
    input sub,
    output [31:0] sum
);
assign b1=b^sub;
wire [15:0]s1,s2;
wire carryp,cout;
add16 a1(a[15:0],b[15:0],sub,s1,carryp);
add16 a2(a[31:16],b[31:16],carryp,s2,cout);

endmodule
