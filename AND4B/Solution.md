```
Inputs: in1[4], in2[4];
Outputs: out[4];

// 1. specify the components you want to use here
Parts:
  myAnd1 AND,
  myAnd2 AND,
  myAnd3 AND,
  myAnd4 AND;

// 2. wire them up
Wires:
  in1[1] -> myAnd1.in1,
  in1[2] -> myAnd2.in1,
  in1[3] -> myAnd3.in1,
  in1[4] -> myAnd4.in1,
  in2[1] -> myAnd1.in2,
  in2[2] -> myAnd2.in2,
  in2[3] -> myAnd3.in2,
  in2[4] -> myAnd4.in2,
  myAnd1.out -> out[1],
  myAnd2.out -> out[2],
  myAnd3.out -> out[3],
  myAnd4.out -> out[4];
```
![AND4B](https://github.com/MasterZydra/MHDR/blob/master/AND4B/AND4B.png?raw=true)
