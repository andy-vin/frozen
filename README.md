#### Frozen literal

#### 1. Object ID
- when true

    input
    ```bash
    > ruby object_id_with_frozen.rb
    ```
    output
    ```bash
    > 60
    > 60
    ```
- when absent

    input
    ```bash
    > ruby object_id_without_frozen.rb
    ```
    output
    ```bash
    > 60
    > 80
    ```
#### 2. Change object

- when true
  
  input
    ```bash
    > ruby change_object_with_frozen.rb
    ```
  output
    ```bash
    > Traceback (most recent call last):
	>         1: from change_object_with_frozen.rb:8:in `<main>'
    > change_object_with_frozen.rb:5:in `change_str': can't modify frozen String: "John" (FrozenError)
    ```
- when absent
  
  input
    ```bash
    > ruby change_object_without_frozen.rb
    ```
  output
    ```bash
    > John Dou
    ```
