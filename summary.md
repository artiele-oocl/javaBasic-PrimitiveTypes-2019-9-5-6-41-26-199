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

#### should_round_number
1. Familiarity with rounding methods. I used class Math.
2. The test failed because it is expected rounded value of type long.
3. I corrected it that way because this specific Math.round expects a double and returns long. No type casting needed.
4. None.

## IntegerTypeTest
#### should_get_range_of_primitive_int_type
1. Familiarity with class Integer's possible max and min values.
2. Test failed because 0 is neither max nor min value for integer.
3. I corrected it that way because I am familiar that there exist a class Integer. And this class describes both behavior
and properties of Integer. I explored and found such methods.
4. None.

#### should_get_range_of_primitive_short_type
1. The same knowledge point as above.
2. Test failed because 0 is neither max nor min for short primitive data type.
3. Same concept as above but this time I explored class Short.
4. None.

#### should_get_range_of_primitive_long_type
1. Same as above.
2. Same as above.
3. Same as above only this time class Long is explored.
4. None.

#### should_get_range_of_primitive_byte_type
1. Same as above.
2. Same as above.
3. Same as above only this time class Byte is explored.
4. None.

#### should_overflow_silently
1. Knowledge is about integer overflow.
https://dzone.com/articles/overflow-and-underflow-data
2. Test failed because 0 is not the integer result after overflow.
3. I answered it this way because when an integer overflows, it simply rolls back to integer minimum value.
I used a property of wrapper class Integer to represent minimum value of integer.
4. None.

#### should_underflow_silently
1. Same as above but this time underflow.
2. Same as above but this time underflow.
3. Just the opposite of overflow where a decrement to integral min would result to rolling back to the max integer
represented by property Integer.MAX_VALUE of wrapper class Integer.
4. None.

#### should_throw_exception_when_overflow
1. Knowledge point is about invoking exception.
2. Test failed because there was no add() implementation.
3. I used bitwise OR operator so I do not need to check variable right when variable left is already integer max. 
4. None.

#### just_prevent_lazy_implementation
1. This is just a happy case scenario for add() implementation.
2. Test failed because there was no add() implementation.
3. I used bitwise OR operator so I do not need to check variable right when variable left is already integer max. 
4. None.

#### should_take_care_of_number_type_when_doing_calculation
1. This is familiarity with Java Math Operator Precedence, and delta paramater of JUnit
http://tutorials.jenkov.com/java/math-operators-and-math-class.html
https://junit.org/junit4/javadoc/4.12/org/junit/Assert.html#assertEquals(double,%20double,%20double)
2. Test failed because expectedResult1 and expectedResult2 is far beyond the marginal error delta.
3. I followed correct math operation precedence.
4. None.

#### should_truncate_number_when_casting
1. This is familiarity with converting integer to short type.
https://www.tutorialspoint.com/java/lang/integer_shortvalue.htm
2. Test failed because it is not equal to the given value.
3. I utilized a method from wrapper class Integer.
4. None.

#### should_increment
1. This is about pre and post incrementation.
http://www.c4learn.com/java/java-increment-decrement-operator/
2. Test failed because zero is not equal to the expected.
3. This test executed post-incrementation where we assigned initial value first then increment that is why expectedResult
is the initial value.
4. None.

#### should_increment_2
1. Same as above.
http://www.c4learn.com/java/java-increment-decrement-operator/
2. Same as above.
3. Same as above but this time pre-incrementation.
4. None.