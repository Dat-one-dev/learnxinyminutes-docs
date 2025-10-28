---
name: Miniscript
contributors:
    - ["DatOneDev", "https://github.com/Dat-one-dev"]
filename: learnminiscript.ms
---

MiniScript is a modern, elegant, and easy-to-learn scripting
language designed to be embedded in other applications.
It's free, open-source, and has been under continuous development since 2016.
You can use MiniScript in standalone tools like Mini Micro and Soda
for game development. Thanks to community plugins, it also integrates with
popular engines like Godot, Unity, Raylib, and MonoGame.
With a clean syntax reminiscent of Python and Lua, its main
advantages are ease of use and tight engine integration.
This makes it a perfect choice for developers just starting
their game development journey.

## Basics

```Miniscript
// Single-line comments are written using slash symbol.

//Variables decelration
i = 8 //Integer
f = 1.2 //Float
b = true //Bool
s = "Hello, World!" //String
l = [1, false, "Dev"] // List - similar to Python,
// it can hold different types
// of variables at once.

m = {1:"one", 2:"two", 3:"three"}
// Map holds key-value pairs.

// Functions
foo = function()
end function //Must end with end function

add = function(first, second) //takes 2 parameters
	return first + second    // return keyword
	//returns any value
	//back to function call
end function

// Increases the Score
score = 0
score += 1
//Decrease the score
score -= 1
// Opperators such as *=, /= and %= can be also used
// These operators is just shorthand of
// score = score + 1

// Printing values
printing = function()
	print "I " + "love " + "Miniscript " + 2 //Miniscript
	//Allows mix of Data types
end function
//Prininting mutliple data types at onceis totally
//doable in Miniscript
//Pranthese can be used in function but its not the
//Intended way Miniscript should be coded
//Instead you can do the most in Minsicript
//without Prathese, expect some scenarios

// Math
doing_math = function()
	first = 8
	second = 4
	print first + second // 12
	print first - second // 4
	print first * second // 32
	print first / second // 2
	print first % second // 0
	print first ^ second // 4096
end function

//Comparison
compare = function()
	print 5 == 5// true  - equal to
	print 5 != 3// true  - not equal to
	print 5 > 3 // true  - greater than
	print 5 < 10// true  - less than
	print 5 >= 5// true  - greater than or equal to
	print 5 <= 4 // false - less than or equal to
	print "apple" == "apple"// true
	print "apple" != "banana"// true
	print "apple" < "banana"// true ("apple" comes first)
	print "zebra" > "apple"// true ("zebra" comes after)
end function

// Control flow
control_flow = function()
	x = 3
	y = 8.2
	y = 2 // y was originally a float,
	// but we can change its type to int
	// using the power of dynamic typing!

	if x < y then //then keyword is required
		print "x is smaller than y"
	else if x > y then
		print "x is bigger than y"
	else
		print "x and y are equal"
	end if //end if keyword is must

	if not x == y then print "X and Y are not same"
	//This is short if-else block, In this
	//end if block can be skipped
	a = true
	b = false
	c = false
	if a and b or not c then
		//And returns true
		//When all values
		//are true
		//Or returns true
		//When one of
		//The value is
		//true
		print "This is true!"
	end if

	for i in range(0, 20)
		print i //Prints from 0 to 20
	end for

	for i in ["two", 3, 1.0]
		print i //Prints the array
	end for

	x = 12
	y = 1

	while x > y
		print y
		y += 1
	end while

	x = 2
	y = 10
	while x > y
		print y
		y += 1
		if y == 7 then break
		//Break keyword exits the loop
	end while
	//end while ends a while block
	//Simmilairy end for ends a
	//for block
	//Same refers to a function
	//block and if-else block
end function
```

## Further Reading

* [Miniscript Offical Website](https://miniscript.org/)
* [Miniscript Wiki](https://miniscript.org/wiki/)
* [Intro to Programming Book](https://introtocomputerprogramming.online/#cover)
* [MiniMicro CheatSheet](https://miniscript.org/files/MiniMicro-CheatSheet.pdf)
* [Miniscript Manual](https://miniscript.org/files/MiniScript-Manual.pdf)
