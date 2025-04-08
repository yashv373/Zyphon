// this example talks about creating modules/sub-modules which then further tell us how to connect them
module ckt20 ( input a, input b, output out );
mod_a a1(.in1(a),.in2(b),.out(out));
endmodule
module mod_a ( input in1, input in2, output out );
    // Module body
endmodule