```
Inputs: in;
Outputs: out;

// 1. specify the components you want to use here
Parts: myNand NAND;

// 2. wire them up
Wires:
  in -> myNand.in1,
  in -> myNand.in2,
  myNAND.out -> out;
```
![NOT](https://github.com/MasterZydra/MHDR/blob/master/NOT/NOT.png?raw=true)
