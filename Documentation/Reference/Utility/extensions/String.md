**EXTENSION**

# `String`

## Methods
<details><summary markdown="span"><code>init(argument:)</code></summary>

```swift
public init(argument: String) throws
```

</details>

<details><summary markdown="span"><code>chomp(separator:)</code></summary>

```swift
public func chomp(separator: String? = nil) -> String
```

> Remove trailing newline characters. By default chomp removes
> all trailing \n (UNIX) or all trailing \r\n (Windows) (it will
> not remove mixed occurrences of both separators.

</details>

<details><summary markdown="span"><code>chuzzle()</code></summary>

```swift
public func chuzzle() -> String?
```

> Trims whitespace from both ends of a string, if the resulting
> string is empty, returns `nil`.String
>
> Useful because you can short-circuit off the result and thus
> handle “falsy” strings in an elegant way:
>
>     return userInput.chuzzle() ?? "default value"

</details>

<details><summary markdown="span"><code>split(around:)</code></summary>

```swift
public func split(around delimiter: String) -> (String, String?)
```

> Splits string around a delimiter string into up to two substrings
> If delimiter is not found, the second returned substring is nil

</details>

<details><summary markdown="span"><code>mangledToBundleIdentifier()</code></summary>

```swift
public func mangledToBundleIdentifier() -> String
```

> Returns a form of the string that is a valid bundle identifier

</details>

<details><summary markdown="span"><code>mangledToC99ExtendedIdentifier()</code></summary>

```swift
public func mangledToC99ExtendedIdentifier() -> String
```

> Returns a form of the string that is valid C99 Extended Identifier (by
> replacing any invalid characters in an unspecified but consistent way).
> The output string is guaranteed to be non-empty as long as the input
> string is non-empty.

</details>

<details><summary markdown="span"><code>mangleToC99ExtendedIdentifier()</code></summary>

```swift
public mutating func mangleToC99ExtendedIdentifier()
```

> Mangles the contents to a valid C99 Extended Identifier.  This method
> is the mutating version of `mangledToC99ExtendedIdentifier()`.

</details>