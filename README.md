# SudokuSolver
#from Sublime Text

#Create a board

board= [
    [7,8,0,4,0,0,1,2,0],
    [6,0,0,0,7,5,0,0,9],
    [0,0,0,6,0,1,0,7,8],
    [0,0,7,0,4,0,2,6,0],
    [0,0,1,0,5,0,9,3,0],
    [9,0,4,0,6,0,0,0,5],
    [0,7,0,3,0,0,0,1,2],
    [1,2,0,0,0,7,4,0,0],
    [0,4,9,2,0,6,0,0,7]
    ]

def print_board(bo):
	for i in range(len(bo)):
		if i%3==0 and i !=0:
			print("------------------------")

	for j in range(len([bo])):
		if j%3 == 0 and j!=0:
			print("|", end= "")

			if j==8:
				print(bo[i][j])
			else:
				print(str(bo[i][j]) + " ", end="")
			#essentially means, stay on the same line when we keep printing things 

def find_empty(bo):
	for i in range(len(bo)):
		for j in range(len(bo[0])):
			if bo[i][j]==0:
				return (i, j) #row, col ... usually he says it's col, row(in porgramming?)
	return none
#try and except?
#backtracking? (Tech W Tim)
#try and except= Naive algorithm
#very slow
#inefficient

#part 2
