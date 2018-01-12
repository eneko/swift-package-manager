**ENUM**

# `ArgumentParserError`

**Contents**

- [Cases](#cases)
  - `unknownOption`
  - `invalidValue`
  - `expectedValue`
  - `unexpectedArgument`
  - `expectedArguments`

```swift
public enum ArgumentParserError: Swift.Error
```

> Errors which may be encountered when running argument parser.

## Cases
### `unknownOption`

```swift
case unknownOption(String)
```

> An unknown option is encountered.

### `invalidValue`

```swift
case invalidValue(argument: String, error: ArgumentConversionError)
```

> The value of an argument is invalid.

### `expectedValue`

```swift
case expectedValue(option: String)
```

> Expected a value from the option.

### `unexpectedArgument`

```swift
case unexpectedArgument(String)
```

> An unexpected positional argument encountered.

### `expectedArguments`

```swift
case expectedArguments(ArgumentParser, [String])
```

> Expected these positional arguments but not found.
