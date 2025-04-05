module top_module(
    input [31:0] a,
    input [31:0] b,
    output [31:0] sum
);
wire c2,c3cout;
wire [15:0] s1,s2,s2;
add16 a1(a[15:0],b[15:0],1'b0,s1,cout);
add16 a2(a[31:16],b[31:16],1'b0,s2,c2);
add16 a3(a[31:16],b[31:16],1'b1,s3,c3);
//2:1mux
always@(*) begin
case(s2,s3)
1'b00:
1'b01:
1'b10:
1'b11:
endcase
end
endmodule
