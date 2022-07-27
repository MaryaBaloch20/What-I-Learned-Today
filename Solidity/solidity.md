## **Solidty**

Solidity is described as a contract. A contract is the primary and essential block of information, used to build all Ethereum applications. This means that all functions, variables have to be defined inside the contract and will define how the contract works.

### **Version**

Solidity source files can contain any number of contract definitions. Each Solidity file also includes a thing called “Version Pragma”. It is used to prevent the code from being compiled with future compiler versions that might introduce incompatible changes. Most of the time, the definition looks like this:

```
	pragma solidity ^0.4.20;
```

In the example above `0.4.20` is the desired compiler version.

### **Contracts**

Now, let’s put it into code.

Contracts in Solidity are similar to classes in object-oriented languages. They contain data in variables and functions that can modify these variables.

They are defined by using a `contract` keyword, followed by the contract name and and two brackets `{ }` which will later enclose contract variables and functions. For example:

```
contract Pizza {

}
``` 

## ****Variables****

### **Variable types**

State variables are used to store information on the blockchain. They can also be manipulated by the functions within the contract.

Solidity is a statically typed programming language, meaning that each variable must have its type specified. Examples of the main data types:

### **Booleans**

Can only have one of the two following values: `true` or `false`. The keyword for Booleans is `bool`.

### **Integers**

Integers can be split into main groups: regular integers (can store both positive and negative values) and unsigned integers (can only store values that are 0 or higher)

Regular integer has keywords from `int8` to `int256`. The number signifies the maximum number of bits it can store (thus limiting the maximum value), and it can be any number between 8 and 256 as long as it incremented in steps of 8 (e.g., `int16` is valid but `int17` is not). The `int` keyword alone would be understood as `int256`.

Unsigned integers follow the same logic. The only difference is the keyword which ranges from `uint8` to `uint256`. Keyword `uint` can also be used instead of `uint256`.

### **Addresses**

The `address` keyword is used to hold Ethereum addresses. If you're planning to store an Ethereum address, you will need to use the `address` keyword.

### **Strings**

The `string` variable is used to store text information. If you need to store a variable that should contain text information use the `string` keyword.