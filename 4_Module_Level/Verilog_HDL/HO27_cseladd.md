module ckt27(
    input [31:0] a,
    input [31:0] b,
    output [31:0] sum
);
wire c2,c3,cout;
wire [15:0] s1,s2,s3;
add16 a1(a[15:0],b[15:0],1'b0,s1,cout);
add16 a2(a[31:16],b[31:16],1'b0,s2,c2);
add16 a3(a[31:16],b[31:16],1'b1,s3,c3);
//2:1mux
always@(*) begin
case(cout)
1'b0: sum={s2,s1};
1'b1: sum={s3,s1};
default: sum={16'b0,s1};
endcase
end
endmodule
