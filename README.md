# FULL_ADDER
# Aim:
To simulate and synthesis the full adder using verilog.
# apparatus Required:
Vivado Xilinx 14.7 Spartan 6 FPGA>
# Procedure:
```
STEP 1: Start the vivado software and select the name and the project.
STEP 2: Select the device family, device, package and speed.
STEP 3: Select new source in the new project and select verilog module as the source type.
STEP 4: Type the file name and module name and click next and then finish button. Type the code and save it.
STEP 5: Select the run simulation and then run behavioural simulation in the source window and click the check syntax.
STEP 6: Click the simulation to stimulate the program and give the inputs and verify the outputs as per the truth table.
STEP 7: Compare the output with the truth table.
```

# Truth Table
![image](https://github.com/RESMIRNAIR/FULL_ADDER/assets/154305926/02ead8f5-d958-4c89-ac51-368ca086cf41)
# Circuit Diagram
![image](https://github.com/RESMIRNAIR/FULL_ADDER/assets/154305926/418e00aa-ed19-4ab3-a413-bae9575bff0e)
![image](https://github.com/RESMIRNAIR/FULL_ADDER/assets/154305926/0c26fe47-d78c-43dd-ac0d-804e427a3bbc)

# Program:
```
module FA (a,b,c,sum,carry);
input a,b,c;
output sum,carry;
wire w1,w2,w3;
xor g1 (w1,a,b);
and g2 (w2,a,b);
xor g3 (sum,w1,c);
and g4 (w3,w1,c);
or g5 (carry,w3,w2);
endmodule
```
# Output:

![full adder](https://github.com/GauravSunehl/FULL_ADDER/assets/166976407/a21dcb23-ca81-4ae2-9c42-23362f1b7986)
# Result:
Thus the verilog program for full adder has been simulated and verified successfully.

