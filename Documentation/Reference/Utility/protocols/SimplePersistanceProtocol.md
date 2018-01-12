**PROTOCOL**

# `SimplePersistanceProtocol`

```swift
public protocol SimplePersistanceProtocol: class, JSONSerializable
```

> A protocol which needs to be implemented by the objects which can be
> persisted using SimplePersistence

## Methods
<details><summary markdown="span"><code>restore(from:)</code></summary>

```swift
func restore(from json: JSON) throws
```

> Restores state from the given json object.

</details>

<details><summary markdown="span"><code>restore(from:supportedSchemaVersion:)</code></summary>

```swift
func restore(from json: JSON, supportedSchemaVersion: Int) throws
```

> Restores state from the given json object and supported schema version.

</details>