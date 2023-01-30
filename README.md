# 同步音律喵赛克 Steam端 存档解析工具
## 界面展示

![主页面](./ReadmeResources/main.png "主页面")

## 更新日志
### Version 1.0.7
1. #### 新增 排除空谱面
    1. 排除0935号谱面ID 原因 该编号未被分配
    2. 排除1022号谱面ID 原因 该编号未被分配
    2. 排除1194号谱面ID 原因 该编号未被分配
    2. 排除1283号谱面ID 原因 该编号未被分配
    2. 排除1342及更高的谱面ID 原因 该编号未被分配
2. #### 修复 歌曲收藏功能异常
    游戏中"收藏"功能仅标记4K Easy难度，目前实现自动对其他难度在分析文件中同时添加标记
3. #### 修复 打开错误的`SavAnalyze.json`文件导致异常闪退的问题
    现在将会自动删除错误文件并重新生成
    如果生成错误，有可能会再次闪退

### 再次申明：妾身`不会`对存档文件进行`写`操作

### Version 1.0.6
1. #### 新增 通过"云端同步率"计算"综合同步率"
2. #### 更改 排序控件
    1. "本地同步率"改为"云端同步率"
3. #### 更改 筛选控件
    1. "Score>122%"改为"黑Ex"
    2. "Score>120%"改为"红Ex"

### Version 1.0.5
1. #### 新增 谱面排序功能
    - 灰色(#F0F0F0)表示未启用该排序方法
    - 绿色(#98E22B)表示已启用该排序的倒序方法
    - 红色(#FF7B7B)表示已启用该排序的正序方法
    1. 按 游玩次数 排序
    2. 按 难度等级 排序
    3. 按 本地同步率 排序
    1. 按 名称 排序
2. #### 新增 谱面筛选按钮增加背景颜色启用标识
    - 灰色(#F0F0F0)表示未启用该筛选方法
    - 绿色(#98E22B)表示已启用该筛选方法
3. #### 新增 谱面筛选功能与谱面排序功能可同时使用
4. #### 更改 筛选控件与排序控件的排版大幅度改动

### Version 1.0.4
1. #### 新增 双击谱面打开新窗口爬取全球数据(未找到排行榜链接)
2. #### 更新 "SongName.json"文件
3. #### 新增 谱面难度等级列
3. #### 更改 谱面难度列分拆为"键数"列和"难度"列

### Version 1.0.3
1. #### 更新 "SongName.json"文件
2. #### 新增 启动状态指示Label

### Version 1.0.2
2. #### 更改 窗口宽高自动识别频率为200ms
1. #### 新增 新版本提示颜色闪烁，改变时间为500ms
3. #### 新增 自动从GitHub Repo获取"./SongName.json"文件
4. #### 新增 自动从"FileExport.py"释放"霞鹜文楷等宽"字体和图标文件

### Version 1.0.1
1. #### 新增 开发者Label和更新获取通道
1. #### 新增 前往GitHub页面的Button
1. #### 新增 第二次及之后的分析会自动读取"./SavAnalyze.json"分析缓存
1. #### 新增 通过读取"./SongName.json"来填充"./SavAnalyze.json"中`SongName`字段

### Version 1.0.0
1. #### 新增 简易自动搜索存档文件
    首次运行时自动搜索每个磁盘的
    1. `./Program Files/steam/steamapps/common/MUSYNX/SavesDir/savedata.sav`
    2. `./SteamLibrary/steamapps/common/MUSYNX/SavesDir/savedata.sav`
    3. `./steam/steamapps/common/MUSYNX/SavesDir/savedata.sav`
    三个目录
2. #### 新增 可以按固定方式筛选谱面
    1. `筛选出 已游玩`
    2. `筛选出 未游玩`
    3. `筛选出 已收藏`
    4. `筛选出 成绩大于122%(即黑EX)`
    5. `筛选出 成绩大于120%(即红EX)`
    6. `按Rank评级: EX、S、A、B、C筛选`
3. #### 新增 允许使用"打开存档"按钮进行文件选择
4. #### 新增 显示当前已筛选出的谱面数量
5. #### 新增 使用红色"重新分析"按钮清除分析缓存并重新生成
6. #### 新增 窗口控件自动跟随窗口大小改变
7. #### 新增 在窗口标题栏显示最后一次游玩曲名