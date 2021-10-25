### Approaches

##### Object serialization of class
1 . First you make a structure (in C# class).
2 . Then make an instance / object of the structure.
3 . Then you can serialize the object into JSON or whatever.


##### Translating object model to structured data
Simple use custom encoder that reads your object/data and transforms it into a different format (CSV, XML etc).