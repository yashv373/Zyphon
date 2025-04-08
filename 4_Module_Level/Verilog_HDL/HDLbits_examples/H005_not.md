// now lets try and model logic gates in verilog.
module ckt5( input in, output out );
assign out=~in; // the ~ operator tells that out should be bar of in, that is , the not of input.
endmodule