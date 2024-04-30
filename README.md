# D_FLIPFLOP
![image](https://github.com/RESMIRNAIR/D_FLIPFLOP/assets/154305926/4f3e1d9d-e0c3-464e-b0e4-e47946c813bd)
# Truth Table
![image](https://github.com/RESMIRNAIR/D_FLIPFLOP/assets/154305926/42d38f79-9cc3-4b09-a46f-e0c1241dee57)

VERILOG CODE
``````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````
module sr_ff(clk,q,rst,s,r); input s,r,clk,rst; output reg q; always@(posedge clk) begin if(rst==1) q=1'b0; else begin case({s,r}) 
2'b00:q=q; 
2'b01:q=1'b0; 
2'b10:q=1'b1; 
2'b11:q=1'bx; 
endcase end end 
endmodule
````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````
OUTPUT

![image](https://github.com/YEMANTHKUMAR/D_FLIPFLOP/assets/160569469/1b1c9252-3010-4d96-b5b9-a2aaad24e796)
