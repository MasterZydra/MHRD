```
Inputs: in1, in2;
Outputs: out, carry;

// 1. specify the components you want to use here
Parts:
  myNandCon NAND,
  myNand1 NAND,
  myNand2 NAND,
  myNandO NAND,
  myNotC NOT;

// 2. wire them up
Wires:
  in1 -> myNandCon.in1,
  in2 -> myNandCon.in2,
  myNandCon.out -> myNotC.in,
  myNotC.out -> carry,
  myNandCon.out -> myNand1.in1,
  myNandCon.out -> myNand2.in1,
  in1 -> myNand1.in2,
  in2 -> myNand2.in2,
  myNand1.out -> myNandO.in1,
  myNand2.out -> myNandO.in2,
  myNandO.out -> out;
```
![XOR](https://github.com/MasterZydra/MHDR/blob/master/HALFADDER/HALFADDER.png?raw=true)
