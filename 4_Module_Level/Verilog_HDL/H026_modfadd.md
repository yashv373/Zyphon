module top_module (
    input [31:0] a,
    input [31:0] b,
    output [31:0] sum
);

endmodule

  
module add1 ( input a, input b, input cin, output sum, output cout );
sum=a^b^cin;
cout=(a&cin)|(b&cin)|(a&b);
endmodule