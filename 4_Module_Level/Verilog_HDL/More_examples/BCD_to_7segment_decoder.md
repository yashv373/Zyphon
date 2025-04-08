Design Code:
```
module bcd_to_7seg (
    input [3:0] bcd,
    output reg [6:0] seg
);
    always @(*) begin
        case (bcd)
            4'd0: seg = 7'b1000000;
            4'd1: seg = 7'b1111001;
            4'd2: seg = 7'b0100100;
            4'd3: seg = 7'b0110000;
            4'd4: seg = 7'b0011001;
            4'd5: seg = 7'b0010010;
            4'd6: seg = 7'b0000010;
            4'd7: seg = 7'b1111000;
            4'd8: seg = 7'b0000000;
            4'd9: seg = 7'b0010000;
            default: seg = 7'b1111111;
        endcase
    end
endmodule

```

Testbench:
```
module bcd_to_7seg_tb;
    reg [3:0] bcd;
    wire [6:0] seg;

    bcd_to_7seg dut (.bcd(bcd), .seg(seg));

    initial begin
        bcd = 0;
        repeat (12) begin
            #10 bcd = bcd + 1;
        end
        #20 $finish;
    end
endmodule

```

Design Constraints (.sdc):
```

```