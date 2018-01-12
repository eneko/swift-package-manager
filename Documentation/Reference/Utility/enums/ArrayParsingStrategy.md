**ENUM**

# `ArrayParsingStrategy`

**Contents**

- [Cases](#cases)
  - `oneByOne`
  - `upToNextOption`
  - `remaining`

```swift
public enum ArrayParsingStrategy
```

> An enum representing the strategy to parse argument values.

## Cases
### `oneByOne`

```swift
case oneByOne
```

> Will parse only the next argument and append all values together: `-Xcc -Lfoo -Xcc -Lbar`.

### `upToNextOption`

```swift
case upToNextOption
```

> Will parse all values up to the next option argument: `--files file1 file2 --verbosity 1`.

### `remaining`

```swift
case remaining
```

> Will parse all remaining arguments, usually for executable commands: `swift run exe --option 1`.
