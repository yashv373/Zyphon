module ckt24 ( 
    input clk, 
    input [7:0] d, 
    input [1:0] sel, 
    output [7:0] q 
);
wire x,y,z;
my_dff8 dff1(.clk(clk),.d(d),.q(x));
my_dff8 dff2(.clk(clk),.d(x),.q(y));
my_dff8 dff3(.clk(clk),.d(y),.q(z));
always