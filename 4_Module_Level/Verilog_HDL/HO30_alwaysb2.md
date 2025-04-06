// synthesis verilog_input_version verilog_2001
module ckt30(
    input clk,
    input a,
    input b,
    output wire out_assign,
    output reg out_always_comb,
    output reg out_always_ff   );
//assign_xor
assign out_assign=a^b;
//always_comb_xor
    always@(*) begin
       out_always_comb=a^b;
    end 
//always_seq_xor
    always@(posedge clk) begin
  out_always_ff<=a^b;
    end
endmodule