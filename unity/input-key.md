# キー入力を取得

## Input.GetAxis()

```cs
Input.GetAxis("Horizontal")
Input.GetAxis("Vertical")
```
 * 矢印キーとWASDキーに対応
 * -1 ~ 1 のfloat値が取得できる
 * キーの押し込みによって値が変わる

## Input.GetKey()

```cs
if (Input.GetKey(KeyCode.W)) {
}
```
 * Booleanが返る
