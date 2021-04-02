
```ruby
# about_arrays.rb
def test_slicing_arrays
  array = [:peanut, :butter, :and, :jelly]
  # why it's that
  assert_equal [], array[4,0]
  assert_equal nil, array[5,0]
end
```

```ruby
  def test_changing_hashes
    hash = { :one => "uno", :two => "dos" }
    hash[:one] = "eins"

    expected = { :one => "eins", :two => "dos" }
    assert_equal expected, hash

    # Bonus Question: Why was "expected" broken out into a variable
    # rather than used as a literal?
  end
```