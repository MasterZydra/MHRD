```
Inputs: in1[4], in2[4], sel;
Outputs: out[4];

// 1. specify the components you want to use here
Parts:
  notSel NOT,
  nandIn1 NAND4B,
  nandIn2 NAND4B,
  nandOut NAND4B;

// 2. wire them up
Wires:
  in1 -> nandIn1.in1,
  in2 -> nandIn2.in1,
  sel -> notSel.in,
  sel -> nandIn2.in2,
  notSel.out -> nandIn1.in2,
  nandIn1.out -> nandOut.in1,
  nandIn2.out -> nandOut.in2,
  nandOut.out -> out;
```
![MUX4B](https://github.com/MasterZydra/MHDR/blob/master/MUX/MUX.png?raw=true)
