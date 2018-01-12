**PROTOCOL**

# `StringEnumArgument`

```swift
public protocol StringEnumArgument: ArgumentKind
```

> A protocol which implements ArgumentKind for string initializable enums.
>
> Conforming to this protocol will automatically make an enum with is
> String initializable conform to ArgumentKind.

## Methods
<details><summary markdown="span"><code>init(rawValue:)</code></summary>

```swift
init?(rawValue: String)
```

</details>