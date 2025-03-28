//Given an 8-bit input vector [7:0], reverse its bit ordering.


module ckt17( 
    input [7:0] in,
    output [7:0] out
);
int i,j;
always@(*) begin
 for (i = 0, j = 7; i < 8; i = i + 1, j = j - 1) begin
        out[j] = in[i];  
    end
end
endmodule