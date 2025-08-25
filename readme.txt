using v1.16.3 and erlang 26; check with "asdf help" -> asdf current

elixir types:
list    []
atom    :name
tuple   {}
map     %{key: value}   
    usage: 
        iex> xy = %{a: "b"}
        iex> xy.a
        "b"

    matching:
        iex> %{a: myvar} = xy
        iex> myvar
        "b"

    update:
        a)
        iex> xy = Map.put(xy, :a, "c")

        b)
        iex> xy = %{ xy | a: "c" }

keyword list
    [ key: value ]
    usage:
        iex> kw = [a: "b"]
        iex> kw[:a]
        "b"
    
    matching:
        iex> [a: myvar] = kw
        iex> myvar
        "b"

struct
    like map, but only defined keys are allowed
 



creating a project:
> mix new identicon
 
start elixir interactive shell in context of your project
> iex -S mix

using ex_doc:
> mix docs

running tests:
> mix test

