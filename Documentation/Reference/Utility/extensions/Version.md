**EXTENSION**

# `Version`

## Properties
<details><summary markdown="span"><code>hashValue</code></summary>

```swift
public var hashValue: Int
```

</details>

<details><summary markdown="span"><code>description</code></summary>

```swift
public var description: String
```

</details>

## Methods
<details><summary markdown="span"><code>==(_:_:)</code></summary>

```swift
static public func == (lhs: Version, rhs: Version) -> Bool
```

#### Parameters

| Name | Description |
| ---- | ----------- |
| lhs | A value to compare. |
| rhs | Another value to compare. |

</details>

<details><summary markdown="span"><code><(_:_:)</code></summary>

```swift
public static func < (lhs: Version, rhs: Version) -> Bool
```

#### Parameters

| Name | Description |
| ---- | ----------- |
| lhs | A value to compare. |
| rhs | Another value to compare. |

</details>

<details><summary markdown="span"><code>init(string:)</code></summary>

```swift
init?(string: String)
```

> Create a version object from string.
>
> - Parameters:
>   - string: The string to parse.

#### Parameters

| Name | Description |
| ---- | ----------- |
| string | The string to parse. |

</details>

<details><summary markdown="span"><code>init(stringLiteral:)</code></summary>

```swift
public init(stringLiteral value: String)
```

#### Parameters

| Name | Description |
| ---- | ----------- |
| value | The value of the new instance. |

</details>

<details><summary markdown="span"><code>init(extendedGraphemeClusterLiteral:)</code></summary>

```swift
public init(extendedGraphemeClusterLiteral value: String)
```

#### Parameters

| Name | Description |
| ---- | ----------- |
| value | The value of the new instance. |

</details>

<details><summary markdown="span"><code>init(unicodeScalarLiteral:)</code></summary>

```swift
public init(unicodeScalarLiteral value: String)
```

#### Parameters

| Name | Description |
| ---- | ----------- |
| value | The value of the new instance. |

</details>

<details><summary markdown="span"><code>init(json:)</code></summary>

```swift
public init(json: JSON) throws
```

</details>

<details><summary markdown="span"><code>toJSON()</code></summary>

```swift
public func toJSON() -> JSON
```

</details>