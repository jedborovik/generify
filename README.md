generify
========

Add Java style generics to ruby collections

```bash
> array = Array.new.generify(String)
> array << "Cheese"
["Cheese"]
> array << 5
Error: Array 'array' only accepts objects of type String
```
