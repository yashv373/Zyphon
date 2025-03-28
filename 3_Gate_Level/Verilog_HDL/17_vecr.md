//Given an 8-bit input vector [7:0], reverse its bit ordering.


module ckt17( 
    input [7:0] in,
    output [7:0] out
);
int i,j;

for(i=0;i<=7,i++)
for(j=7;j>=0;j--)
assign out[j]=in[i];

endmodule