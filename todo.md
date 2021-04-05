
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

```ruby
  def test_method_names_become_symbols
    symbols_as_strings = Symbol.all_symbols.map { |x| x.to_s }
    assert_equal true, symbols_as_strings.include?("test_method_names_become_symbols")
    assert_equal true, Symbol.all_symbols.include?(:test_method_names_become_symbols)
  end

  # THINK ABOUT IT:
  #
  # Why do we convert the list of symbols to strings and then compare
  # against the string value rather than against symbols?

  # It's important to realize that symbols are not "immutable
  # strings", though they are immutable. None of the
  # interesting string operations are available on symbols.

  # THINK ABOUT IT:
  #
  # Why is it not a good idea to dynamically create a lot of symbols?
```

https://stackoverflow.com/questions/13661193/ruby-scopes-constants-precedence-lexical-scope-or-inheritance-tree


```ruby
  # THINK ABOUT IT:
  #
  # The two major ways to write class methods are:
  #   class Demo
  #     def self.method
  #     end
  #
  #     class << self
  #       def class_methods
  #       end
  #     end
  #   end
  #
  # Which do you prefer and why?
  # Are there times you might prefer one over the other?
```

```ruby
    # THINK ABOUT IT:
    #
    # Why does Ruby provide both send and __send__ ?
```
