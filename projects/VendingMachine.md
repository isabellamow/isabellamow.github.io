---
layout: project
type: project
image: img/Screenshot 2026-01-29 215055.png
title: "Vending Machine"
date: 2024
published: true
labels:
  - Java
  - Data Structures
  - Object-Oriented Programming
summary: "A vending machine system written in Java that helps you add, find and print snacks."
---

<div class="text-center p-4">
  <img width="200px" src="../img/micromouse/micromouse-robot.png" class="img-thumbnail" >
  <img width="200px" src="../img/micromouse/micromouse-robot-2.jpg" class="img-thumbnail" >
  <img width="200px" src="../img/micromouse/micromouse-circuit.png" class="img-thumbnail" >
</div>

At Leeward Community College, ICS 211: Computer Science II has students complete a cumulative project that recreates a vending machine. It utilizes concepts that we have learned throughout the class such as binary trees and linking. The vending machine is organized so that each node holds one snack and references two other nodes. The vending machine allows you to add, find, and print snacks. Each snack consists of a barcode, name, number of calories, and price. The entire vending machine uses a binary search tree architecture combined with custom node and interface classes. 

The vending machine project helped me learn how to program to an interface and the distinction between what a node does and how it performs. Becuase this project included custom error handling, input validation, and encpasulation, I was able to build foundational computer science skills and practice real world system modeling.

Here is some code that illustrates how I went about creating the object construction and validation logic:

```cpp
//private class variables
public class Snack {
  private int barcode;
  private int calories;
  private double price;
  private String name;

//snack(int ibarcode, int icalories, double dprice, String sname)
  //constructor with same parameters as given by assignment
  //has throw exception because set methods could have an exception due to invalid input
  public Snack(int barcode, int calories, double price, String name) throws SnackException { 
    this.setBarcode(barcode);
    this.setName(name); 
    this.setCalories(calories); 
    this.setPrice(price); 
  }

  //set barcode and put constraints according to assignment to check for valid user input. 
  //Throws snack exception and two print statements if it is not valid. This. statement to assign user input to barcode. 
  public void setBarcode(int barcode) throws SnackException {
    if (barcode < 10001 || barcode > 99999) { 
      System.out.println("Barcode must be between 10001 and 99999.");
      throw new SnackException("Not a valid barcode");
    }
    this.barcode = barcode; //used to change the class variable to inputed barcode 
  }

```
