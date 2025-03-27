# COP2664-1-Lesson-7-Programming-Assignment
This repository link is a submission link for COP2664-1: Lesson 7 Programming Assignment

import UIKit
class Calculator : NSObject
{
    func AddTwoNumbers(firstNumber:Double, secondNumber:Double) -> Double {
      return firstNumber + secondNumber
    }
    func SubtractTwoNumbers(firstNumber:Double, secondNumber:Double) -> Double {
        return firstNumber - secondNumber
    }
    func MulitplyTwoNumbers(firstNumber:Double, secondNumber:Double) -> Double {
        return firstNumber * secondNumber
    }
    func DivideTwoNumbers(firstNumber:Double, secondNumber:Double) -> Double? {
        if (secondNumber == 0) {
            return nil
        }
        return firstNumber / secondNumber
    }
}

var arithmeticCalculator:Calculator = Calculator()
let num1 = 17.5
let num2 = 19.76
let sum = arithmeticCalculator.AddTwoNumbers(firstNumber: num1, secondNumber: num2)
let difference = arithmeticCalculator.SubtractTwoNumbers(firstNumber: num1, secondNumber: num2)
let product = arithmeticCalculator.MulitplyTwoNumbers(firstNumber: num1, secondNumber: num2)
let division = arithmeticCalculator.DivideTwoNumbers(firstNumber: num1, secondNumber: num2)

print("\num1) + \(num2) is \(sum)")
print("\num1) - \(num2) is \(difference)")
print("\(num1) * \(num2) is \(product)")
print("\num1) / \(num2) is \(division!)")
