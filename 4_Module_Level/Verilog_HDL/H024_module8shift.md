module ckt24 ( 
    input clk, 
    input [7:0] d, 
    input [1:0] sel, 
    output reg [7:0] q 
);
wire [7:0] x, [7:0]y, [7:0]z;
my_dff8 dff1(.clk(clk),.d(d),.q(x));
my_dff8 dff2(.clk(clk),.d(x),.q(y));
my_dff8 dff3(.clk(clk),.d(y),.q(z));
always@(clk,d,x,y,z) begin
case(sel)
2'b00: q=d;
2'b01: q=x;
2'b10: q=y;
2'b11: q=z;
default: q="undefined";
endcase