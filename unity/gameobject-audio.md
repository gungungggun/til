# ぶつかった時に音を鳴らす

```cs
public AudioClip audioClip1;
private AudioSource audioSource;

private void OnCollisionEnter(Collision collision)
{
    audioSource = gameObject.GetComponent<AudioSource>();
    audioSource.clip = audioClip1;
    audioSource.Play();
}
```

音源ファイルはゲームオブジェクトの中に入れておく必要がある
