https://hdlbits.01xz.net/mw/images/3/3a/Wiredecl2.png
// we need to implement the above circuit
// source HDLbits: Implement the following circuit. Create two intermediate wires (named anything you want) to connect the AND and OR gates together. Note that the wire that feeds the NOT gate is really wire out, so you do not necessarily need to declare a third wire here. Notice how wires are driven by exactly one source (output of a gate), but can feed multiple inputs.

module ckt(
    input a,
    input b,
    input c,
    input d,
    output out,
    output out_n   ); 
wire a1,a2,a3;
    assign a1=a&b;
    assign a2=c&d;
    assign a3=a1|a2;
    // or a3=a&b|c&d;
    assign out=a3;
    assign out_n=~a3;
endmodule