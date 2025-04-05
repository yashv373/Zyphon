// this example talks about creating modules/sub-modules which then further tell us how to connect them
module top_module ( input a, input b, output out );
endmodule
module top_module(.a(in1),.b(in2),.out(out));
endmodule