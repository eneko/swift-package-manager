**PROTOCOL**

# `ArgumentParserProtocol`

```swift
public protocol ArgumentParserProtocol
```

> Argument parser protocol passed in initializers of ArgumentKind to manipulate
> parser as needed by the argument.

## Properties
<details><summary markdown="span"><code>currentArgument</code></summary>

```swift
var currentArgument: String
```

> The current argument being parsed.

</details>

<details><summary markdown="span"><code>associatedArgumentValue</code></summary>

```swift
var associatedArgumentValue: String?
```

> The associated value in a `--foo=bar` style argument.

</details>

## Methods
<details><summary markdown="span"><code>next()</code></summary>

```swift
mutating func next() -> String?
```

> Provides (consumes) and returns the next argument. Returns `nil` if there are not arguments left.

</details>

<details><summary markdown="span"><code>peek()</code></summary>

```swift
func peek() -> String?
```

> Peek at the next argument without consuming it.

</details>