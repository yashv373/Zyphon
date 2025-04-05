module ckt25(
    input [31:0] a,
    input [31:0] b,
    output [31:0] sum
);
parameter cin=1'b0;
wire cintrm,cout;
wire [15:0] s1,s2;
add16 a1(a[15:0],b[15:0],cin,s1,cintrm);
add16 a2(a[31:16],b[31:16],cintrm,s2,cout);
assign sum={s2,s1};
endmodule