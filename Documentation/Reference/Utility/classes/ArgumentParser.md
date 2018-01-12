**CLASS**

# `ArgumentParser`

**Contents**

- [Methods](#methods)
  - `init(commandName:usage:overview:seeAlso:)`
  - `add(option:shortName:kind:usage:completion:)`
  - `add(option:shortName:kind:strategy:usage:completion:)`
  - `add(positional:kind:optional:usage:completion:)`
  - `add(positional:kind:optional:strategy:usage:completion:)`
  - `add(subparser:overview:)`
  - `parse(_:)`
  - `printUsage(on:)`

```swift
public final class ArgumentParser
```

> Argument parser struct responsible to parse the provided array of arguments
> and return the parsed result.

## Methods
<details><summary markdown="span"><code>init(commandName:usage:overview:seeAlso:)</code></summary>

```swift
public init(commandName: String? = nil, usage: String, overview: String, seeAlso: String? = nil)
```

> Create an argument parser.
>
> - Parameters:
>   - commandName: If provided, this will be substitued in "usage" line of the generated usage text.
>   Otherwise, first command line argument will be used.
>   - usage: The "usage" line of the generated usage text.
>   - overview: The "overview" line of the generated usage text.
>   - seeAlso: The "see also" line of generated usage text.

#### Parameters

| Name | Description |
| ---- | ----------- |
| commandName | If provided, this will be substitued in “usage” line of the generated usage text. Otherwise, first command line argument will be used. |
| usage | The “usage” line of the generated usage text. |
| overview | The “overview” line of the generated usage text. |
| seeAlso | The “see also” line of generated usage text. |

</details>

<details><summary markdown="span"><code>add(option:shortName:kind:usage:completion:)</code></summary>

```swift
public func add<T: ArgumentKind>(
        option: String,
        shortName: String? = nil,
        kind: T.Type,
        usage: String? = nil,
        completion: ShellCompletion? = nil
    ) -> OptionArgument<T>
```

> Adds an option to the parser.

</details>

<details><summary markdown="span"><code>add(option:shortName:kind:strategy:usage:completion:)</code></summary>

```swift
public func add<T: ArgumentKind>(
        option: String,
        shortName: String? = nil,
        kind: [T].Type,
        strategy: ArrayParsingStrategy = .upToNextOption,
        usage: String? = nil,
        completion: ShellCompletion? = nil
    ) -> OptionArgument<[T]>
```

> Adds an array argument type.

</details>

<details><summary markdown="span"><code>add(positional:kind:optional:usage:completion:)</code></summary>

```swift
public func add<T: ArgumentKind>(
        positional: String,
        kind: T.Type,
        optional: Bool = false,
        usage: String? = nil,
        completion: ShellCompletion? = nil
    ) -> PositionalArgument<T>
```

> Adds an argument to the parser.
>
> Note: Only one positional argument is allowed if optional setting is enabled.

</details>

<details><summary markdown="span"><code>add(positional:kind:optional:strategy:usage:completion:)</code></summary>

```swift
public func add<T: ArgumentKind>(
        positional: String,
        kind: [T].Type,
        optional: Bool = false,
        strategy: ArrayParsingStrategy = .upToNextOption,
        usage: String? = nil,
        completion: ShellCompletion? = nil
    ) -> PositionalArgument<[T]>
```

> Adds an argument to the parser.
>
> Note: Only one multiple-value positional argument is allowed.

</details>

<details><summary markdown="span"><code>add(subparser:overview:)</code></summary>

```swift
public func add(subparser command: String, overview: String) -> ArgumentParser
```

> Add a parser with a subcommand name and its corresponding overview.

</details>

<details><summary markdown="span"><code>parse(_:)</code></summary>

```swift
public func parse(_ arguments: [String] = []) throws -> Result
```

> Parses the provided array and return the result.

</details>

<details><summary markdown="span"><code>printUsage(on:)</code></summary>

```swift
public func printUsage(on stream: OutputByteStream)
```

> Prints usage text for this parser on the provided stream.

</details>