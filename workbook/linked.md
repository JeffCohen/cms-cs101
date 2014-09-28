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
puts colors.size # 7
puts colors[3]   # green

# bonus
puts colors.to_s  # "red, orange, yellow, green, blue, indigo, violet"
colors.delete("green")
puts colors.size    # 6
puts colors.to_s  # "red, orange, yellow, blue, indigo, violet"
