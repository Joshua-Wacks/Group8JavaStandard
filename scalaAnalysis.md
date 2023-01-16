# Group 8's Scala Language Analysis

## High-level Overview
  Scala is a pure object-oriented language in the sense that every value is an object and every function is a value. 
  It is a statically and strongl-typed language.
  Scala is a compiled language wherein everything gets compiled to byte-code and runs within the JVM (it also has Javascript runtimes).


## Data-types
## Primitive Types
  Double, Float, Long, Int, Short, Byte, Char, Unit and Boolean(all are non-nullable except for Unit).
  
## Composite Types
  Tuples and Arrays as well as Union and Intersection types
  
## Collection Types
  Sequences, maps and sets( and all thier different implementations)
  
## Coercion, Conversion & Casting
  A = B.asInstanceOf[class];
  where, 
  A is the object to which the casted instance of B is returned, 
  B is the object to be casted, 
  and class is the name of the class to which B is to be casted into.
  
## Iterators and Generators
  for elem <- it do println(elem)         //Example of for each loop
  it.foreach(println)                     //Example of iterator 
  while it.hasNext do println(it.next())  //Example of iterator 
  
  def example = generator[Any] {produce =>
    produce( "first" )
    for( i <- suspendable(1 until 4)) 
        produce(i) 
    produce("last")
    }
    for( a <- example ) 
        println(a)                       //Example of generator(works the same as yield in Python
        
## Constants
  The val refers to a constant and var refers to a variable.
  
 ##Immutable Values(Scalas baseline is that the varaibles are immutable and we need to specify if we want a variable to be mutable)
  In Scala; with functions, function arguments are val by default, so no extra typing is needed.
  In Scala, all number types, strings, and tuples are immutable.

## Statements vs Expressions
  println("Hello Scala")
  // Output:- Hello Scala
  //The above line of code is a statement.
  
  var x = 2 * Math.sqrt(10) / 5
  // Output:- x: Double = 1.2649110640673518
  //The above line of code is an expression.

## Unique Features
   It can be used along with Java as it runs on the JVM (it can import Java libraries and vice versa).
   It has 'match expressions' which can be used like switch cased
   
 ## Pattern Matching
   Scala does support patter matching and can be implemented as follows:
   def examine[T](seq: Seq[T]): Seq[String] = seq map {
          case i: Int => s"Int: $i"
          case other => s"Other: $other"
        }
    case i: Int => s"Int: $i"

## 'Destructuring' Sugar
  This works using the import keyword
  case class Abc(a: Int, b: Int, c: Int)
  val obj = Abc(1, 2, 3)
  val somethingUsingOnlyAandC = {
    import obj.{a, c}
    a + c
  }

  println(somethingUsingOnlyAandC) // Output: 4
  
 ## Imperative vs Declarative For Summation

  val values = Array.fill[Double](numValues)(0) // Imperative

  val sumOfValues = values.sum // Declerative
  
 ## For Filtering and Grouping
  df.groupBy("x").count()
  .filter("count >= 2")
  .show() //Declerative

 ## Date-types
  In scala we do not have any inherent date-time libraries or functions available, but we can use java data time, calendar, Date library to deal with dates
  
 ## Size of Int
  Cannot specify the size of a datatype but BigInt and other types are supported.
 
