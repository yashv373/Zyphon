// this example talks about creating modules/sub-modules which then further tell us how to connect them
module top_module ( input a, input b, output out );
mod_a ( input in1, input in2, output out );
endmodule
module mod_a ( input in1, input in2, output out );
    // Module body
endmodule