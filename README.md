# lk

## README.md
####  README.md


https://github.com/lk80231314/lk/blob/7fbf523e7d71f6fc4202678675fae065b0a5e1b0/lk1

---


网络图片：

![网络图片](https://ss0.bdstatic.com/70cFuHSh_Q1YnxGkpoWK1HF6hhy/it/u=4208887636,142271560&fm=26&gp=0.jpg)



---


文件夹下的图片:

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
    @Override
    public void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.main);
        TextView text = (TextView) findViewById(R.id.text_Info);
        text.setTextColor(Color.GREEN);
        text.setText("欢迎使用百度地图Android SDK v" + VersionInfo.getApiVersion());
        setTitle(getTitle() + " v" + VersionInfo.getApiVersion());
        ListView mListView = (ListView) findViewById(R.id.listView);
        // 添加ListItem，设置事件响应
        mListView.setAdapter(new DemoListAdapter());
        mListView.setOnItemClickListener(new OnItemClickListener() {
            public void onItemClick(AdapterView<?> arg0, View v, int index, long arg3) {
                onListItemClick(index);
            }
        });

        // 申请动态权限
        requestPermission();

        // 注册 SDK 广播监听者
        IntentFilter iFilter = new IntentFilter();
        iFilter.addAction(SDKInitializer.SDK_BROADTCAST_ACTION_STRING_PERMISSION_CHECK_OK);
        iFilter.addAction(SDKInitializer.SDK_BROADTCAST_ACTION_STRING_PERMISSION_CHECK_ERROR);
        iFilter.addAction(SDKInitializer.SDK_BROADCAST_ACTION_STRING_NETWORK_ERROR);
        mReceiver = new SDKReceiver();
        registerReceiver(mReceiver, iFilter);
    }

    
    ```
