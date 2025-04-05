// You are given a module named `mod_a` that has 2 outputs and 4 inputs, in that order. You must connect the 6 ports _by position_ to your top-level module's ports `out1`, `out2`, `a`, `b`, `c`, and `d`, in that order.
//module mod_a ( output, output, input, input, input, input );
module ckt21 ( 
    input a, 
    input b, 
    input c,
    input d,
    output out1,
    output out2
);
mod_a a1 (out1,out2,a,b,c,d);
endmodule
