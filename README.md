generify
========

Add Java style generics to ruby collections

###Array
```bash
> array = Array.new.generify(String)
=> []
> array << "Cheese"
=> ["Cheese"]
> array << 5
Error: Array 'array' only accepts objects of type String
```
###Hash
```bash
> hash = Hash.new.generify_key(Symbol).generify_value(Fixnum)
=> {}
> hash[:first] = 1
=> 1
> hash["second"] = 2
Error: Hash 'hash' only accepts keys of type Symbol
> hash[:second] = "2"
Error: Hash 'hash' only accepts values of type Fixnum
