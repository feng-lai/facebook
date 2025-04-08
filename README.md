# Facebook 爬虫使用说明

## 1. 安装依赖库

```bash
pip install -r requirements.txt
```

## 2. 配置 `facebook.py`

### 填写账号密码
在代码的指定位置填写您的 Facebook 账号和密码：

```python
# 示例代码（替换引号内的内容）
username = "your_username"
password = "your_password"
```

### 替换小组链接
将代码中的链接替换为您要爬取的目标小组链接：

```python
# 示例代码（替换为实际小组链接）
group_url = "https://www.facebook.com/groups/your_target_group"
```

### 设置爬取数量（可选）
如果需要限制爬取的数据量，修改以下两处的数字：

```python
# 示例代码（修改数字为所需数量）
while len(data) < 98:
```
```python
# 示例代码（修改数字为所需数量）
if len(data) >= 98:
```

## 3. 处理手动操作情况

### 弹窗关闭
如果出现以下弹窗，请手动点击关闭：
[![1.png](https://i.postimg.cc/Gt1LCdJn/1.png)](https://postimg.cc/2b2RdpK0)
[![2.png](https://i.postimg.cc/9FbW63Ds/2.png)](https://postimg.cc/F7f5SBgx)

### 刷新页面
如果出现页面加载问题，请手动点击刷新：
[![3.png](https://i.postimg.cc/CKBSnzcV/3.png)](https://postimg.cc/v1sppHRP)

### 验证码处理
如果遇到图片验证码，请按页面提示填写，程序会继续运行不会退出。

## 4. 完成提示
当看到以下输出时表示爬取完成：
```python
"Data saved to .......csv"
```

