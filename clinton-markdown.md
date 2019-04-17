# Classes and Objects


## How to create a class

A class is created simply by typing class followed by the name of that class. Class names use camel case, meaning that words must always be capitalised with no spaces as opposed to lower case words with underscores in between. 

For example: 

``` ruby
class Person
```

## what is an attribute? 

Classes have attributes which are also known as instance variables, these only apply to the *instance* or *object* that they have been applied to. Attributes must be initialised and this can be done in the following way.

``` ruby
def initialize(name, weight)
    @name = name
    @weight = weight
end
```

## How can attributes be accessed? 

Class attributes begin as a private object and can be accessed by using getters and setters. You can give *read only* access *write only* access or *read and write* access. You can write these as seperate methods below your initialize method as below: 

Getter:
``` ruby
def get_player_name
        @player_name
end
```
Setter:
```ruby
 def set_player_name(player_name)
        @player_name = player_name
end
```
An easier way to do this is to use Ruby's in built functions which are a short hand way of doing the above fast and conveniently: 
```ruby
attr_reader(:name, :weight)
attr_writer(:name, :weight)
```
or you can give read and write access in the on simple line using attr_accessor:
``` ruby
attr_accessor(:name, :weight)
```

To read more about accessors click this link: [Ruby's attr_accessor, attr_reader and attr_writer](https://mixandgo.com/learn/ruby_attr_accessor_attr_reader_attr_writer "An article about accessors")

## How do i create an instance of a class? 

This is super easy! all you have to do is create an instance as a variable and pass a new instance of the class to that variable making sure you include the relevant attribures that you have deemed necessary:

```ruby
person1 = Person.new("Geoff", "100 kilograms")
```

once a person is created we can then print out their name and weight as follows: 
```ruby
print person1.name
print person1.weight
```
## So what have we learned today? 

1. What a class is
2. How to make a class
3. How to initialise the attributes of a class
4. How to access the attributes of that class
5. How to create and instance or object of a class
6. How to print out the instance variables of a class. 

![a picture for no reason](https://imagesvc.timeincapp.com/v3/mm/image?url=https%3A%2F%2Ftimedotcom.files.wordpress.com%2F2014%2F11%2Fpotato.jpg&w=800&c=sc&poi=face&q=85 "Here is an image of a potato for no reason")