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

3.Set

