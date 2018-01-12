**CLASS**

# `Result`

**Contents**

- [Properties](#properties)
  - `description`
- [Methods](#methods)
  - `get(_:)`
  - `get(_:)`
  - `get(_:)`
  - `get(_:)`
  - `subparser(_:)`

```swift
public class Result: CustomStringConvertible
```

> A class representing result of the parsed arguments.

## Properties
<details><summary markdown="span"><code>description</code></summary>

```swift
public var description: String
```

</details>

## Methods
<details><summary markdown="span"><code>get(_:)</code></summary>

```swift
public func get<T>(_ argument: OptionArgument<T>) -> T?
```

> Get an option argument's value from the results.
>
> Since the options are optional, their result may or may not be present.

</details>

<details><summary markdown="span"><code>get(_:)</code></summary>

```swift
public func get<T>(_ argument: OptionArgument<[T]>) -> [T]?
```

> Array variant for option argument's get(_:).

</details>

<details><summary markdown="span"><code>get(_:)</code></summary>

```swift
public func get<T>(_ argument: PositionalArgument<T>) -> T?
```

> Get a positional argument's value.

</details>

<details><summary markdown="span"><code>get(_:)</code></summary>

```swift
public func get<T>(_ argument: PositionalArgument<[T]>) -> [T]?
```

> Array variant for positional argument's get(_:).

</details>

<details><summary markdown="span"><code>subparser(_:)</code></summary>

```swift
public func subparser(_ parser: ArgumentParser) -> String?
```

> Get the subparser which was chosen for the given parser.

</details>