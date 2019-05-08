```
Inputs: in, sel;
Outputs: out1, out2;

// 1. specify the components you want to use here
Parts:
  nand1 NAND,
  nand2 NAND,
  not1 NOT,
  not2 NOT;

// 2. wire them up
Wires:
  sel -> nand2.in2,
  in -> nand1.in1,
  in -> nand2.in1,
  nand2.out -> nand1.in2,
  nand2.out -> not2.in,
  not2.out -> out2,
  nand1.out -> not1.in,
  not1.out -> out1;
```
![DEMUX](https://github.com/MasterZydra/MHDR/blob/master/DEMUX/DEMUX.png?raw=true)
![DEMUX](https://github.com/MasterZydra/MHDR/blob/master/DEMUX/DEMUX_Opt.png?raw=true)
