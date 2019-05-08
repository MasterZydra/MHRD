```
Inputs: in1, in2, sel;
Outputs: out;

// 1. specify the components you want to use here
Parts:
  nandSel NAND,
  nandIn1 NAND,
  nandIn2 NAND,
  nandOut NAND;

// 2. wire them up
Wires:
  in1 -> nandIn1.in1,
  in2 -> nandIn2.in1,
  sel -> nandSel.in1,
  sel -> nandSel.in2,
  sel -> nandIn2.in2,
  nandSel.out -> nandIn1.in2,
  nandIn1.out -> nandOut.in1,
  nandIn2.out -> nandOut.in2,
  nandOut.out -> out;
```
![MUX](https://github.com/MasterZydra/MHDR/blob/master/MUX/MUX.png?raw=true)
