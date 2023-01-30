# Design-and-stimulate-8-1-MUX-using-verilog
## AIM:
To determine the design and stimulate 8:1 multiplexer using verilog.

## HARDWARD REQUIRED:
– PC, Cyclone II , USB flasher.

## SOFTWARD REQUIRED:
Quartus prime.

## PROCEDURE:
### Step 1:
Open Quartus II and select new project and choose the file location.

### Step 2:
Module Declaration. Module should have the file name.

### Step 3:
Declare Inputs and outputs.

### Step 4:
Use assign declaration and wire to define the functionality of logic circuits.

### Step 5:
End the program with endmodule.

### Step 6:
Run the program and choose RTL viewer to get RTL realization.

## PROGRAM:
```
module mux8_1(d0,d1,d2,d3,d4,d5,d6,d7,s0,s1,s2,out);
input wire d0,d1,d2,d3,d4,d5,d6,d7,s0,s1,s2;
output reg out;
always@(*)
begin
case(s0 & s1 & s2)
3'b000: out=d0;
3'b001: out=d1;
3'b010: out=d2;
3'b011: out=d3;
3'b100: out=d4;
3'b101: out=d5;
3'b110: out=d6;
3'b111: out=d7;
default: out=1'b0;
endcase
end
endmodule
```

## OUTPUT:
![output](/nameout1.png)
![output](/nameout2.png)
![output](/nameout3.png)

## RESULT:
Design and stimulate 8:1 multiplex is obtained by using verilog code.