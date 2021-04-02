
```ruby
# about_arrays.rb
def test_slicing_arrays
  array = [:peanut, :butter, :and, :jelly]
  # why it's that
  assert_equal [], array[4,0]
  assert_equal nil, array[5,0]
end
```

