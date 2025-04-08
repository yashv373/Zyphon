module ckt23 (
input clk, d
output q
);
wire x,y;
my_dff dff1(.clk(clk),.d(d),.q(x));
my_dff dff2(.clk(clk),.d(x),.q(y));
my_dff dff3(.clk(clk),.d(y),.q(q));
endmodule