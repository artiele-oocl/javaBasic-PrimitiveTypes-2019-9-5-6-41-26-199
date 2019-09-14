# Summary

Please answer the following 4 questions for each unit test:
1. What is the knowledge point of the test? Where is the official document to the knowledge point?
2. Why the test failed at first?
3. Why you corrected the test that way?
4. Do you have further questions on this knowledge point?

## BooleanOperatorsTest
#### should_perform_logical_boolean_operations
1. This test is about relational, bitwise, and logical operators commonly used in Java.
https://www.javatpoint.com/operators-in-java
2. The test failed because expectedResult should be an array of boolean values with 14 elements.
3. Test is corrected that way because test name should_perform_logical_boolean_operations indicates that we perform
logical boolean operations.
4. None.

#### should_do_bitwise_and_boolean_operation
1. This test is about familiarity of 3 famous number systems: hexadecimal, binary, and decimal.
It is also an application of performing bitwise operations. To perform bitwise operations, I had to
represent given hex to binary. Since the given hex are not simple, I find a way to convert them online.
https://www.binaryhexconverter.com/hex-to-binary-converter
https://www.binaryhexconverter.com/binary-to-decimal-converter
2. The test failed because the operation will not yield integer 0.
3. I corrected the test by converting the hex to binary first then performing boolean operation because only binary
can be used for boolean operations.
4. None.

#### should_do_bitwise_or_boolean_operation
1. This test is about familiarity of 3 famous number systems: hexadecimal, binary, and decimal.
It is also an application of performing bitwise operations. To perform bitwise operations, I had to
represent given hex to binary. Since the given hex are not simple, I find a way to convert them online.
https://www.binaryhexconverter.com/hex-to-binary-converter
https://www.binaryhexconverter.com/binary-to-decimal-converter
2. The test failed because the operation will not yield integer 0.
3. I corrected the test by converting the hex to binary first then performing boolean operation because only binary
can be used for boolean operations.
4. None.

#### should_do_bitwise_not_operation
1. This test is about familiarity of 3 famous number systems: hexadecimal, binary, and decimal.
It is also an application of performing bitwise operations. To perform bitwise operations, I had to
represent given hex to binary. Since the given hex are not simple, I find a way to convert them online.
https://www.binaryhexconverter.com/hex-to-binary-converter
https://www.binaryhexconverter.com/binary-to-decimal-converter
https://www.baeldung.com/java-bitwise-operators
2. The test failed because the operation will not yield integer 0.
3. I corrected the test by converting the hex to binary first then performing boolean operation bitwise complement.
First, get all 1's complement by flipping all bits resulting to 1111 1111 1111 1111. Then, since left most bit is one,
this means that value is negative and I need to get its 2's complement by adding one to the 1's complement.
After getting its correct binary values, I convert it back to decimal with a negative sign.
4. None.
