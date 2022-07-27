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