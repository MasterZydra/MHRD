```
Inputs: in1, in2;
Outputs: out;

// 1. specify the components you want to use here
Parts:
  myNot1 NOT,
  myNot2 NOT,
  myNand NAND;

// 2. wire them up
Wires:
  in1 -> myNot1.in,
  in2 -> myNot2.in,
  myNot1.out -> myNand.in1,
  myNot2.out -> myNand.in2,
  myNand.out -> out;
```
![OR](https://github.com/MasterZydra/MHDR/blob/master/OR/OR.png?raw=true)
