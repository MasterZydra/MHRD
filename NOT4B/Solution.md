```
Inputs: in[4];
Outputs: out[4];

// 1. specify the components you want to use here
Parts:
  myNot1 NOT,
  myNot2 NOT,
  myNot3 NOT,
  myNot4 NOT;

// 2. wire them up
Wires:
  in[1] -> myNot1.in,
  in[2] -> myNot2.in,
  in[3] -> myNot3.in,
  in[4] -> myNot4.in,
  myNot1.out -> out[1],
  myNot2.out -> out[2],
  myNot3.out -> out[3],
  myNot4.out -> out[4];
```
![OR](https://gitlab.com/HeinD/MHRD/raw/master/NOT4B/NOT4B.png)