#Data Structure

1.String
  - store string,number
  - `set key value`
	set key-value in redis
  - `get key`
	get the value of key
  - `del key`
	delelte the key-value

2.List
  - `rpush listName item`
	push item from right and return the list's length
  - `lpush listName item`
	push item from left
  - `lpop`
	pop up an element from left and return the value of the element what is popped
  - `rpop`
  - `lindex listName indexNumber`
	* index from 0
	* -1 means the end of the list
	* get the element who's index is indexNumber
  - `lrange listName firstIndex lastIndex`
	get the childList from firstIndex to lastIndex (-1 is the end of the list)
  - only store string element
  - sequential access
  - be able to have the same element

3.Set
  - store string only
  - hash access
  - a key to set,no key for value (element)
  - can not have the same value
  - command
	* `sadd setName value`
		add a element to a set.if add successfully,will return 1.if return 0,means that,it had contained the value.
	* `smembers setName`
		get all the members of an set.
		tips:if the set has large of values.It will be slow.So,be careful when use the function.
	* `sismember setName value1`
		return value1 is a member of a set.If it is,return 1,else return 0.
	* `srem setName value`
		remove a value from a set.
		will return the number of elements which were removed.
