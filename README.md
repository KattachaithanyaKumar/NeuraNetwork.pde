# NeuraNetwork.pde
A java library made in processing (in .pde) made inspired by @Daniel Shiffman(https://github.com/CodingTrain/Toy-Neural-Network-JS) 

note: it is not complete. backpropogation needs to be implemented

## commands

In the Matrix class:
- constructor() : Syntax : new Matrix(rows, cols)
- displayMatrix() : A void function that will print the data in the matrix
- randomize() : A void function that will randomize the value of the data in the matrix (a double value betweem -1 and 1)
- addNum(n) : A void function that will perform scalar addition of a number 'n' to the matrix
- addMatrix(m) : A void function that will add a matrix m to the callers matrix
- multiplyNum(n) : A void function that will perform scalar multiplication of a number 'n' to the matrix
- multiply(b) : A function that returns a matrix after performing multiplication with matrix b with the callers matrix
- transpose() : A function that returns a matrix after performing transpose on the callers matrix

In the NeuralNetwork class:
- constructor() : syntax : new NeuralNetwork(inp_nodes, hidden_nodes, out_nodes)
- feedforward(inp) : A function that returns a output matrix after performing feedforward 
- sigmoid(x): A function that performs sigmoid on a given value used as a activation function

## Using

- in the main.pde (or any other file) create an object for the NeuralNetwork class by giving it the number of input, hidden and output nodes.
- from that object call feedforward(inp) function giving it an array of inputs and store the returned value in a Matrix object.
- using that Matrix object we can call the displayMatrix() function to see what is the guess generated from the network.
