# CompSci-251-Programming-Assignment-2-solution

Download Here: [CompSci 251 Programming Assignment 2 solution](https://jarviscodinghub.com/assignment/compsci-251-programming-assignment-2-solution/)

For Custom/Original Work email jarviscodinghub@gmail.com/whatsapp +1(541)423-7793

1 Overview
For this assignment, you are asked to implement a class which represents a closed, one-dimensional range.
Each range has a minimum and maximum value (where the minimum is always less than or equal to the
maximum). These ranges are closed, meaning that the min and max values are inclusive (belong to the
range).
2 Requirements
You should implement the Range class according to the following UML diagram. Be sure to include a small
comment for at least each non-trivial method.
Range
– min : double
– max : double
+ Range()
+ Range(min: double, max: double)
+ equals(other: Range): boolean
+ toString(): String
+ getMin() : double
+ getMax() : double
+ setMin(min: double)
+ setMax(max: double)
+ setRange(min: double, max: double)
+ contains(point: double): boolean
+ contains(other: Range): boolean
+ intersects(other: Range): boolean
+ union(other: Range): Range
+ intersection(other: Range): Range
The default (no-argument) constructor should initialize both member variables to 0.0. If the two-argument
constructor receives invalid parameters (max < min), then both member variables should also be initialized to 0.0. 1 The equals method should return true if the member variables of this and other are equivalent. The toString method should return a string representation of the object with the form Range(min, max) where min and max are replaced by values of the appropriate member variables. The setters (including setRange) should not change the values of the member values if it would become invalid. For example, setting the min of Range(1.0, 3.0) to 4.0 would not modify the range object. The contains method should return true if the point or range is completely contained within the range represented by this and false otherwise. For example, Range(1.0, 5.0) contains Range(2.0, 3.0) but not Range(4.0, 6.0). The intersects method should return true if there is a non-empty overlap between two range objects. For example, Range(1.0, 5.0) intersects with Range(5.0, 6.0) but not Range(6.0, 7.0). The union method should return the smallest range which completely covers both range objects this and other. There may be a gap between the two ranges, which will also be covered by the resulting range. The union of Range(1.0, 3.0) and Range(4.0, 6.0) is Range(1.0, 6.0) and the union of Range(1.0, 5.0) and Range(2.0, 3.0) is Range(1.0, 5.0). The intersection method should return the intersection of two range objects, if it exists. If no intersection exists (if the two ranges do not overlap), then you should return null to signify an invalid object. The intersection of Range(1.0, 5.0) and Range(3.0, 6.0) is Range(3.0, 5.0). There is no intersection between Range(1.0, 2.0) and Range(3.0, 4.0). For all of the methods described above, it is important to remember that the range object is inclusive with respect to the range’s minimum and maximum values. Ignoring this will lead to subtle errors with contains, intersects, union, and intersection methods. You will also be creating a separate driver class (including the main method) which will create instances of Range and manipulate it. All output and user input should be confined within the driver class. The driver should be written to mimic the sample runs on the following pages. If there is any ambiguity please ask for clarification. 3 Submission Submit both Java files in a zip file to the D2L dropbox before the posted deadline. 2 3.1 Sample Run 1 Enter min and max values for Range1: 2 4 Enter min and max values for Range2: 3 6 Range1 = Range(2.0, 4.0) Range2 = Range(3.0, 6.0) Enter new min value for Range1: 5 Enter new max value for Range1: 1 Enter new min and max values for Range2: 4 7 Range1 = Range(2.0, 4.0) Range2 = Range(4.0, 7.0) Enter a point: 5 Range(2.0, 4.0) does NOT contain 5.000000. Range(4.0, 7.0) contains 5.000000. Range(2.0, 4.0) does NOT contain Range(4.0, 7.0). Range(4.0, 7.0) does NOT contain Range(2.0, 4.0). The union of Range(2.0, 4.0) and Range(4.0, 7.0) is Range(2.0, 7.0). The intersection of Range(2.0, 4.0) and Range(4.0, 7.0) is Range(4.0, 4.0). 3.2 Sample Run 2 Enter min and max values for Range1: 3 4 Enter min and max values for Range2: 2 5 Range1 = Range(3.0, 4.0) Range2 = Range(2.0, 5.0) Enter new min value for Range1: 1 Enter new max value for Range1: 4 Enter new min and max values for Range2: 0 10 Range1 = Range(1.0, 4.0) Range2 = Range(0.0, 10.0) Enter a point: 4 Range(1.0, 4.0) contains 4.000000. Range(0.0, 10.0) contains 4.000000. Range(1.0, 4.0) does NOT contain Range(0.0, 10.0). Range(0.0, 10.0) contains Range(1.0, 4.0). The union of Range(1.0, 4.0) and Range(0.0, 10.0) is Range(0.0, 10.0). The intersection of Range(1.0, 4.0) and Range(0.0, 10.0) is Range(1.0, 4.0). 3 3.3 Sample Run 3 Enter min and max values for Range1: 1 2 Enter min and max values for Range2: 5 6 Range1 = Range(1.0, 2.0) Range2 = Range(5.0, 6.0) Enter new min value for Range1: 3 Enter new max value for Range1: 4 Enter new min and max values for Range2: 8 9 Range1 = Range(1.0, 4.0) Range2 = Range(8.0, 9.0) Enter a point: 7 Range(1.0, 4.0) does NOT contain 7.000000. Range(8.0, 9.0) does NOT contain 7.000000. Range(1.0, 4.0) does NOT contain Range(8.0, 9.0). Range(8.0, 9.0) does NOT contain Range(1.0, 4.0). The union of Range(1.0, 4.0) and Range(8.0, 9.0) is Range(1.0, 9.0). The intersection of Range(1.0, 4.0) and Range(8.0, 9.0) does not exist.
