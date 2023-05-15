# hosting
Personal repo to host images to be used in other readme

## Instructions To Run 
### Requirements 
- Python 3.8 and above
- numpy 
- matPlotLib
- sympy
### Triangulation of complex method 
Triangulate the complex and then enter it into the ```Input_Points.txt``` file in the given format(text indicated with ```//``` is for instruction and should NOT be included in the txt file).
```
1 0 0 0 //Point number(1), follwed by x, y and z coordinates(all integer).
2 3 5 7 //Points to which 1 is connected through edges(Neighbourhood points).
2 1 2 4 //Point number(2), follwed by x, y and z coordinates.
1 3 5   //Points to which 2 is connected, note: if 1 is connected to 2, it should be mentioned that 2 is also connected to 1.
3 1 4 5 //Point number(7), follwed by x, y and z coordinates.
1 2 5.  //The neighbourhood should be mentioned in eaither clockwise or anti clockwise manner
4 4 4 1
1 5 6 7
5 2 3 3
3 1 2 4
6 4 4 8
4
7 -1 -1 -1
1 4      //Continue till the last point.
x        // Use 'x' to indicate end of file.
```
The above input represents this complex given in 
Then, on terminal run 
``` bash
python3 main.py
```
Enter choice 1, and then press any charecter and click enter.
This will generate 2 graphs, 1st one is the simplex and second one is the approximate reeb graph along with the critical points marked in colors mentioned in the legend.
