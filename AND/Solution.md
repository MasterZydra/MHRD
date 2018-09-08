```
Inputs: in1, in2;
Outputs: out;

// 1. specify the components you want to use here
Parts:
  myNot NOT,
  myNand NAND
  ;

// 2. wire them up
Wires:
  in1 -> myNand.in1,
  in2 -> myNand.in2,
  myNand.out -> myNot.in,
  myNot.out -> out
  ;
```