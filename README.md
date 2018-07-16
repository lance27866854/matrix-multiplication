# matrix-multiplication

I implement a MM machine using verilog.
The input includes clock, reset and read_data,
while the output includes index of the matrix, read enable, write enable, data, choice of the matrix and finish.
I use four states to process this program: IDEL, READ_SIZE, READ_MATRIX, WRITE.
In the IDEL state, the mission is nothing but to initialize all the variables.
In the READ_SIZE state, the machine reads the information about the size of the matrix stored in the database, and stores them.
In the READ_MATRIX state, according to different i and j the machine gets data from the database, and sums them up.
First, the machine reads the data of matrix A, then reads the matrix B, repeatly.
Second, count how many times the machine has executed. If the count equals to 2 times columns of matrix A, this step ends.
In the WRITE state, comfirm the index of the matrix and write the operated data back to the database.