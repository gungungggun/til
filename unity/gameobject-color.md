# ぶつかった時にゲームオブジェクトの色を変更する

```cs
    private void OnCollisionEnter(Collision collision)
    {
        // スクリプトをいれたゲームオブジェクトの色変更
        gameObject.GetComponent<Renderer>().material.color = Color.blue;

        // スクリプトをいれたゲームオブジェクトに衝突したオブジェクトの色変更
        collision.gameObject.GetComponent<Renderer>().material.color = Color.green;
    }
```
