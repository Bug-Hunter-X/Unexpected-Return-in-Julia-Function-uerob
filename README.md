# Julia Function Bug

This repository demonstrates a subtle bug in a Julia function that can lead to unexpected behavior. The function `my_function` is intended to return the square of its input if the input is positive, and the negative of the square if the input is negative. However, due to an unnecessary `return 0` statement, the function's behavior is unpredictable.  The bug is subtle because the extra `return` is unreachable, but the compiler doesn't necessarily optimize it away, leading to potential issues in some cases.