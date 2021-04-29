# lk

## README.md
####  README.md


if you want to go to test.md
click https://github.com/redrumq/krowemoh/blob/8746e6868f5fc2aa0dc01d5bdb854f7418dd3366/test.md

---


网络图片：

![网络图片](https://ss0.bdstatic.com/70cFuHSh_Q1YnxGkpoWK1HF6hhy/it/u=4208887636,142271560&fm=26&gp=0.jpg)



---


github文件夹下的一张图片:

![avatar](https://github.com/lk80231314/lk/blob/1bfa19c5a8d213115a4f58f288196526710ddb09/QQ%E5%9B%BE%E7%89%8720210429195111.jpg)


---


an externalweb site:
<https://www.baidu.com/>



---




a block quote:
>love
>>me
>>>action
---



 a bulleted list:
+ lk1
+ lk2
+ lk3
+ lk4
+ lk5

---



a numbered list:


1. test1：
    - one
    - two
    
2. test2：
    - three

    
3. test3：
    - four
    
    
 ---
    
 


a table:

| 性别   | 年龄  |
|  ----  | ----  |
| 男  | 21 |
| 女  | 18 |



---


**一二三**

*四五六*

~~七八九~~



---

```java
private void requestPermission() {
        if (Build.VERSION.SDK_INT >= 23 && !isPermissionRequested) {
            isPermissionRequested = true;
            ArrayList<String> permissionsList = new ArrayList<>();
            String[] permissions = {
                    Manifest.permission.ACCESS_NETWORK_STATE,
                    Manifest.permission.INTERNET,
                    Manifest.permission.WRITE_EXTERNAL_STORAGE,
                    Manifest.permission.READ_EXTERNAL_STORAGE,
                    Manifest.permission.ACCESS_COARSE_LOCATION,
                    Manifest.permission.ACCESS_FINE_LOCATION,
                    Manifest.permission.ACCESS_WIFI_STATE,
            };

            for (String perm : permissions) {
                if (PackageManager.PERMISSION_GRANTED != checkSelfPermission(perm)) {
                    permissionsList.add(perm);
                    // 进入到这里代表没有权限.
                }
            }

            if (!permissionsList.isEmpty()) {
                String[] strings = new String[permissionsList.size()];
                requestPermissions(permissionsList.toArray(strings), 0);
            }
        }
    }
    
    ```
