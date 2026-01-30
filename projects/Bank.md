---
layout: project
type: project
image: img/micromouse/micromouse-square.jpg
title: "Bank"
date: 2025
published: true
labels:
  - C++
summary: "A banking system written in C++ that helps you create, print, find, and delete records."
---

<div class="text-center p-4">
  <img width="200px" src="../img/micromouse/micromouse-robot.png" class="img-thumbnail" >
  <img width="200px" src="../img/micromouse/micromouse-robot-2.jpg" class="img-thumbnail" >
  <img width="200px" src="../img/micromouse/micromouse-circuit.png" class="img-thumbnail" >
</div>

At UH Manoa, ICS 212: Program Structure requires two big projects. A banking project completed in C and C++, both written using terminal. This means learning how to compile, link, and run programs directly from the command line. This added an extra element of complexity to this project as learning how to use the terminal tends to have a learning curve. In 212, we also made use of Makefiles, which automated builds. This helped me to gain a better understanding of the software build process. 

This command-line banking system allows users to manage their accounts. This includes the creation of new accounts, searching records, deleting records, and finding specific records. Some of the core features is its ability to save data to a file and load in data from a file when the program starts. The system stores the account records using dynamic data structure.  

This project makes use of modular program design, meaning that the user interface and database are separate. It uses pointers and dynamic memory allocation. This is why the debug mode is helpful in addition to the release mode. In this project, I learned how to manually manage memory in C and C++. I also learned how to design a simple database system. In the future, security measures such as a password and a more developed user interface could improve it.

Here is some code that illustrates how I went about creating the user interface:

```cpp
byte ADCRead(byte ch)
{
    word value;
    ADC1SC1 = ch;
    while (ADC1SC1_COCO != 1)
    {   // wait until ADC conversion is completed   
    }
    return ADC1RL;  // lower 8-bit value out of 10-bit data from the ADC
}
```

