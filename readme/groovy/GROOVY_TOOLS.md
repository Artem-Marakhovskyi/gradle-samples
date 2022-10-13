- Groovy has an interactive mode - groovysh
- https://groovyconsole.appspot.com/ # web sandbox
- https://groovy-lang.org/differences.html   
- both are equivalent
`println ("Hello World");`
`println "Hello World"`

- members are `public` by default
- `return` is optional
- lots of packages are imported
- 'a' == "a" == ```a```
- supports GString type which is interpolable string
`String message = "Hello $name"`
- Everything is an object
  `8.toString()`
  `4.times { // Run a task // }`
  `7.next()`
- Groovy automatically picks the type for numbers
- `def` or type for declaring variables 
- `println list.get(1)`       // Prints second
- `println list.getAt(-1)`    // Prints last
- `list.each { println it }`
- `map = [ "red" : 1 , "yellow" : 2, "green" : 3 ]`


Closures are anonymous functions
`def greet = {String name -> "Hello ${name}" }`
`greet "Joe"`
`greet.call "Joe"`
`def greet = {"Hello"}` #does not take any arguments
`def greet = {"Hello $it"}`
`{ -> }`                     // Empty Closure
`{ a, b -> a + b }`          // Closure with two untyped arguments
`{int a, int b -> a + b}`    // Closure with two arguments of type int