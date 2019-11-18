<h2 align="center" id="qqmusicapi">QQ Music API</h2>

!> QQ音乐API koa2 版本, 通过Web网页版请求QQ音乐接口数据, 有问题请提 [issue](https://github.com/yan123zi/qqMusicApi/issues), 或者你有其他想法欢迎`PR`.

## API结构图

![qq-music](https://raw.githubusercontent.com/yan123zi/testdoc/master/screenshot/qqmusicapi.PNG)

## API接口

!> koa2 接口说明(参数, 地址, 效果图)

### 获取歌单所有分类

接口说明: 调用此接口, 可获取歌单分类, 包含`category`信息

接口地址: `/playList/allCategories`

调用例子: `/playList/allCategories`

<details>
    <summary>SortId</summary>
    
        sortId: 1, sortName: 默认
        sortId: 2, sortName: 最新
        sortId: 3, sortName: 最热
        sortId: 4, sortName: 评分
        sortId: 5, sortName: none
</details>

**歌单分类(categoryId & categoryName)**
<details>
  <summary>1. 热门</summary>

    1.1
      "categoryId": 10000000,
      "categoryName": 全部,
</details>

<details>
  <summary>2. 语种</summary>
  
    2.1
      "categoryId": 167,
      "categoryName": "英语",
    2.2
      "categoryId": 168,
      "categoryName": "韩语",
    2.3
      "categoryId": 166,
      "categoryName": "粤语",
    2.4
      "categoryId": 169,
      "categoryName": "日语",
    2.5
      "categoryId": 170,
      "categoryName": "小语种",
    2.6
      "categoryId": 203,
      "categoryName": "闽南语",
    2.7
      "categoryId": 204,
      "categoryName": "法语",
    2.8
      "categoryId": 205,
      "categoryName": "拉丁语",
</details>

<details>
  <summary>3. 流派</summary>

    3.1
      "categoryId": 6,
      "categoryName": "流行",
    3.2
      "categoryId": 15,
      "categoryName": "轻音乐",
    3.3
      "categoryId": 11,
      "categoryName": "摇滚",
    3.4
      "categoryId": 28,
      "categoryName": "民谣",
    3.5
      "categoryId": 8,
      "categoryName": "R&B",
    3.6
      "categoryId": 153,
      "categoryName": "嘻哈",
    3.7
      "categoryId": 24,
      "categoryName": "电子",
    3.8
      "categoryId": 27,
      "categoryName": "古典",
    3.9
      "categoryId": 18,
      "categoryName": "乡村",
    3.10
      "categoryId": 22,
      "categoryName": "蓝调",
    3.11
      "categoryId": 21,
      "categoryName": "爵士",
    3.12
      "categoryId": 164,
      "categoryName": "新世纪",
    3.13
      "categoryId": 25,
      "categoryName": "拉丁",
    3.14
      "categoryId": 218,
      "categoryName": "后摇",
    3.15
      "categoryId": 219,
      "categoryName": "中国传统",
    3.16
      "categoryId": 220,
      "categoryName": "世界音乐",
</details>

<details>
  <summary>4. 主题</summary>

    4.1
      "categoryId": 39,
      "categoryName": "ACG",
    4.2
      "categoryId": 136,
      "categoryName": "经典",
    4.3
      "categoryId": 146,
      "categoryName": "网络歌曲",
    4.4
      "categoryId": 133,
      "categoryName": "影视",
    4.5
      "categoryId": 141,
      "categoryName": "KTV热歌",
    4.6
      "categoryId": 131,
      "categoryName": "儿歌",
    4.7
      "categoryId": 145,
      "categoryName": "中国风",
    4.8
      "categoryId": 194,
      "categoryName": "古风",
    4.9
      "categoryId": 148,
      "categoryName": "情歌",
    4.10
      "categoryId": 196,
      "categoryName": "城市",
    4.11
      "categoryId": 197,
      "categoryName": "现场音乐",
    4.12
      "categoryId": 199,
      "categoryName": "背景音乐",
    4.13
      "categoryId": 200,
      "categoryName": "佛教音乐",
    4.14
      "categoryId": 201,
      "categoryName": "UP主",
    4.15
      "categoryId": 202,
      "categoryName": "乐器",
    4.16
      "categoryId": 14,
      "categoryName": "DJ",
</details>

<details>
  <summary>5. 心情</summary>

    5.1
      "categoryId": 52,
      "categoryName": "伤感",
    5.2
      "categoryId": 122,
      "categoryName": "安静",
    5.3
      "categoryId": 117,
      "categoryName": "快乐",
    5.4
      "categoryId": 116,
      "categoryName": "治愈",
    5.5
      "categoryId": 125,
      "categoryName": "励志",
    5.6
      "categoryId": 59,
      "categoryName": "甜蜜",
    5.7
      "categoryId": 55,
      "categoryName": "寂寞",
    5.8
      "categoryId": 126,
      "categoryName": "宣泄",
    5.9
      "categoryId": 68,
      "categoryName": "思念",
</details>

<details>
  <summary>6. 场景</summary>

    6.1
      "categoryId": 78,
      "categoryName": "睡前",
    6.2
      "categoryId": 102,
      "categoryName": "夜店",
    6.3
      "categoryId": 101,
      "categoryName": "学习",
    6.4
      "categoryId": 99,
      "categoryName": "运动",
    6.5
      "categoryId": 99,
      "categoryName": "运动",
    6.6
      "categoryId": 76,
      "categoryName": "约会",
    6.7
      "categoryId": 94,
      "categoryName": "工作",
    6.8
      "categoryId": 81,
      "categoryName": "旅行",
    6.9
      "categoryId": 103,
      "categoryName": "派对",
    6.10
      "categoryId": 222,
      "categoryName": "婚礼",
    6.11
      "categoryId": 223,
      "categoryName": "咖啡馆",
    6.12
      "categoryId": 224,
      "categoryName": "跳舞",
    6.13
      "categoryId": 16,
      "categoryName": "校园",
  </summary>
</details>

示例截图:

![获取歌单分类](https://raw.githubusercontent.com/yan123zi/testdoc/master/screenshot/playListCategories.png)

### 获取歌单列表

接口说明：调用此接口，可以获得你想得到的歌单列表

参数列表：

- 必选参数

`categoryId`：类别`id`，默认是10000000

- 可选参数

`limit`：每次取出的歌单数量，默认是19

`offset`：偏移量，默认是0

`sortId`：排序id：2:最新 5:推荐，默认是5

接口地址：`/playList/:categoryId`

调用例子：`/playList/10000000 || /playList?categoryId=10000000`

实例截图：

**获取歌单列表**

![通过分类获取歌单列表](https://raw.githubusercontent.com/yan123zi/testdoc/master/screenshot/playListByCategory.png)

**获取歌单列表-带参数**

![通过分类获取歌单列表-带参数](https://raw.githubusercontent.com/yan123zi/testdoc/master/screenshot/playListByCategoryWithParams.png)

### 获取歌单详情

接口说明：调用此接口，可以获得歌单的详情

参数列表：

- 必选参数

`id`：歌单的id

接口地址：`/playListDetails/:id`

调用例子：`/playListDetails/6375131889`

实例截图：

**获取歌单详情**

![获取歌单详情](https://raw.githubusercontent.com/yan123zi/testdoc/master/screenshot/playListDetails.png)

### 获取歌曲的链接

接口说明：调用该接口，可以获得歌曲的vkey，歌曲外链和一些其它参数

参数列表：

- 必选参数

`id`：歌曲的id

接口地址：`/songUrl/:id`

调用例子：`/songUrl/001Xn6C50lvtLc`

实例截图：

**获取歌曲的链接**

![获取歌曲的链接](https://raw.githubusercontent.com/yan123zi/testdoc/master/screenshot/songUrl.png)

### 获取歌曲的歌词

接口说明：调用该接口，可以获得歌曲的歌词

参数列表：

- 必选参数

`id`：歌曲的id

接口地址：`/songLyric/:id`

调用例子：`/songLyric/231745979`

实例截图：

**获取歌曲的链接**

![获取歌曲的链接](https://raw.githubusercontent.com/yan123zi/testdoc/master/screenshot/songLyric.png)

### 获取歌曲的详情

接口说明：调用该接口，可以获得歌曲的详情

参数列表：

- 必选参数

`id`：歌曲的id

接口地址：`/songDetails/:id`

调用例子：`/songDetails/0035KWhu1mizlY`

实例截图：

**获取歌曲的链接**

![获取歌曲的链接](https://raw.githubusercontent.com/yan123zi/testdoc/master/screenshot/playListDetails.png)

### 获取歌曲的相关mv

接口说明：调用该接口，可以获得歌曲的相关的mv

参数列表：

- 必选参数

`id`：歌曲的id

接口地址：`/songRelateMv/:id`

调用例子：`/songRelateMv/0035KWhu1mizlY`

实例截图：

**获取歌曲的链接**

![获取歌曲的链接](https://raw.githubusercontent.com/yan123zi/testdoc/master/screenshot/songMv.png)