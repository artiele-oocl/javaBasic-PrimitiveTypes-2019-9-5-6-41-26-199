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

## CharTypeTest
#### should_describe_escaped_chars
1. This test is about popular reserved characters that needed to be escaped using backslash in order to be used properly.
https://www.freeformatter.com/java-dotnet-escape.html#ad-output
2. The test failed because those reserved characters do not represent empty spaces.
3. The reserved characters are quite popular.
4. None.

## FloatingTypeTest
#### should_not_get_rounded_result_if_convert_floating_number_to_integer
1. This test is about getting the integer value of a floating number.
https://www.baeldung.com/java-type-casting
2. The test failed because the problem is about getting the integer value of given floating number not getting
the max allowable integer value.
3. I corrected it that way because I only need to get the integer part of the given floating number; no rounding up.
4. None.

#### should_judge_special_double_cases
1. This test is about familiarity with the class Double and its method.
https://www.tutorialspoint.com/java/lang/double_isinfinite.htm
2. The test failed because there were no implementations for both isNan and isInfinity inside the class.
3. I corrected it that way because an already existing static method from class Double can be reused. No need to
reinvent the wheel.
4. None.

#### should_not_round_number_when_convert_to_integer
1. This has the same concept as should_not_get_rounded_result_if_convert_floating_number_to_integer.
2. Test failed because it is not asking for the highest integer value possible.
3. I corrected it that way because it has the same knowledge point as the first test in this class.
4. None.
