---
title:  "Java Cheatsheet"
---
# Primitives

Name    | Size   | Signed | Notes
------- | ------ | ------ | ------
byte    | 8 bit  | ✓      | -128 to 127
short   | 16 bit | ✓      | -32,768 to 32,767
int     | 32 bit | ✓/✗    | -2<sup>31</sup> to 2<sup>31</sup>-1
long    | 64 bit | ✓/✗    | -2<sup>63</sup> to 2<sup>63</sup>-1
float   | 32 bit | ✓      | Floating. Don't use for precise values.
double  | 64 bit | ✓      | Floating.
char    | 16 bit | ✗      | '\u0000' to '\uffff'
boolean | ?      | ✗      | true or false


# Variable assignment

```
type name = value; // Primitives

Class name = new Class(); // Class instances

type[] name = new type[length]; // Arrays

ArrayList<type> name = new ArrayList<>(); // ArrayList
```
