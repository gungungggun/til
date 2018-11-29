# 必ず一定のバウンドをさせる

Physic Materialの設定では一定のバウンドをずっと続けることができない（多分）  
解決策として、Physic Materialは設定せず、スクリプトで衝突したときに固定値で跳ね返す方法がある

```cs
    private Rigidbody rb;

    private void OnCollisionEnter(Collision collision)
    {
        rb.AddForce(Vector3.up * 10f, ForceMode.Impulse);
    }
```


