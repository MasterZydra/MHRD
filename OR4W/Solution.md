```
Inputs: in[4];
Outputs: out;

// 1. specify the components you want to use here
Parts:
  myOr1 OR,
  myOr2 OR;
  myOrE OR;

// 2. wire them up
Wires:
  in[1] -> myOr1.in1,
  in[2] -> myOr1.in2,
  in[3] -> myOr2.in1,
  in[4] -> myOr2.in2,
  myOr1.out -> myOrE.in1,
  myOr2.out -> myOrE.in2,
  myOrE.out -> out;
```
![NOT](https://github.com/MasterZydra/MHDR/blob/master/OR4W/OR4W.png?raw=true)
