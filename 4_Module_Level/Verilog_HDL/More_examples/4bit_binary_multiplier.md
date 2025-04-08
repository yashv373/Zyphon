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

```