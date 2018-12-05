# ゲームオブジェクトをクリックしたとき

## 準備
 * カメラにPhysics Raycaster
 * HierarchyにUI>EventSystem

## Script
``` cs
using System.Collections;
using System.Collections.Generic;
using UnityEngine;
using UnityEngine.EventSystems;

public class click : MonoBehaviour, IPointerClickHandler {

  public void OnPointerClick(PointerEventData eventData)
  {
      Debug.Log("clicked");
  }
}
```
