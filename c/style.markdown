Ars - C Style
=============

* Structure
    * Rules
        * Group local variables by type in start of function, new line after.
        * Group local conditional variables to conditional, no new line after.
        * New line before final return.
        * New line before and after seperate logic.

* Keywords
    * Rules:
        * One space after:
            * Include:
                * `do for if`
        * Parentheses:
            * Include:
                * `sizeof typeof alignof defined (cast)`

* Urnary operators.
    * Rules:
	    * One space after none before.
	        * Include:
                * `post++ post--`
        * One space before none after:
            * Include:
                * `--pre ++pre &  *  +  -  ~  !  sizeof  typeof  alignof  __attribute__  defined`
            * Reasoning:
                * Readability.

* Binary operators.
    * Rules:
        * One space before and after:
            * Include:
                * `= + - * / % == != > < >= <= && || & | ^ << >>`
            * Reasoning:
                * Readability.

* Ternary operators.
    * Rules:
        * One space before and after:
            * Include:
                * `? :`
            * Reasoning:
                * Readability.

* Other operators.
    * Rules:
        * One space after:
            * Include:
                * `[]`
            * Reasoning:
                * Readability.
