Design code
```
module multiplier4 (
    input  [3:0] a,
    input  [3:0] b,
    output [7:0] product
);
    assign product = a * b;
endmodule

```
Testbench
```
module multiplier4_tb;
    reg  [3:0] a, b;
    wire [7:0] product;

    multiplier4 dut (
        .a(a),
        .b(b),
        .product(product)
    );

    initial begin
        $monitor("a=%d, b=%d, product=%d", a, b, product);

        a = 4'd3;  b = 4'd2;   #10; // expected op=6
        a = 4'd7;  b = 4'd5;   #10; // expected op=35
        a = 4'd15; b = 4'd15;  #10; // expected op=225
        a = 4'd8;  b = 4'd4;   #10; // expected op=32
        $finish;
    end
endmodule

```
.sdc file
```
# Create a virtual clock to give STA a reference
create_clock -name virtual_clk -period 3.0

# Set input delays (we're assuming max 1.5ns from source to input ports)
set_input_delay 1.5 -clock virtual_clk [get_ports a]
set_input_delay 1.5 -clock virtual_clk [get_ports b]

# Set output delay (we expect the product to be valid within 1.5ns after processing)
set_output_delay 1.5 -clock virtual_clk [get_ports product]

```