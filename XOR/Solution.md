```
Inputs: in1, in2;
Outputs: out;

// 1. specify the components you want to use here
Parts:
  myNand1 NAND,
  myNand2 NAND,
  myNand3 NAND,
  myNand NAND;

// 2. wire them up
Wires:
  in1 -> myNand1.in1,
  in1 -> myNand2.in1,
  in2 -> myNand2.in2,
  in2 -> myNand3.in2,
  myNand2.out -> myNand1.in2,
  myNand2.out -> myNand3.in1,
  myNand1.out -> myNand.in1,
  myNand3.out -> myNand.in2,
  myNand.out -> out;
```
![XOR](https://github.com/MasterZydra/MHDR/blob/master/XOR/XOR.png?raw=true)
