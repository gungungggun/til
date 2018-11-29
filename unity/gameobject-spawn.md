#  ゲームオブジェクトを一定時間でスポーン

```cs
public class spawn : MonoBehaviour {

  public GameObject spawnObject;
  public float interval = 1f;

  void Start () {
    StartCoroutine("Spawn");
  }

  IEnumerator Spawn() {
    while(true){
      GameObject go = Instantiate(spawnObject, transform.position, Quaternion.identity);
      go.SetActive(true);
      yield return new WaitForSeconds(interval);
    }
  }
}
```
