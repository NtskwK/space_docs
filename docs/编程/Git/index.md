# 版本管理

## 回滚版本

可选参数：
- soft:不保存工作区和暂存区
- hard:保存工作区和暂存区
- mixed:仅保存工作区

```bash
# 上一版本
git reset HEAD^
# 上两个版本
git reset HEAD^^
# 十个版本之前
git reset --hard head~10
# 指定版本
git reset --hard [hash]
```

# 设置代理

## 添加代理

```bash
//http || https
git config --global http.proxy 127.0.0.1:7890
git config --global https.proxy 127.0.0.1:7890

//sock5代理
git config --global http.proxy socks5 127.0.0.1:7891
git config --global https.proxy socks5 127.0.0.1:7891
```

## 取消代理

```bash
git config --global --unset http.proxy
git config --global --unset https.proxy
```