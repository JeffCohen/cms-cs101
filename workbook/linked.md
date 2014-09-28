# Linked List

```ruby
colors = LinkedList.new
colors.add("red")
colors.add("orange")
colors.add("yellow")
colors.add("green")
colors.add("blue")
colors.add("indigo")
colors.add("violet")

# typical
puts colors.size  # 7
puts colors.first # red
puts colors[3]    # green

# bonus 1
puts colors.to_s  # "red, orange, yellow, green, blue, indigo, violet"

# bonus 2
colors.delete("green")
puts colors.size    # 6
puts colors.to_s  # "red, orange, yellow, blue, indigo, violet"
```

## Rules

1. Your LinkedList class may not use include Enumerable or any built-in Ruby class that implements Enumerable.
