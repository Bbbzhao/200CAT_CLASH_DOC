# 自定义节点排序

## 版本要求 <a id="&#x7248;&#x672C;&#x8981;&#x6C42;"></a>

0.9.10版本更新后，支持自定义节点排序

## 配置文件 <a id="&#x914D;&#x7F6E;&#x6587;&#x4EF6;"></a>

在 `config.yaml`（General中点击Text Mode Edit）中添加以下字段:

```text
cfw-proxies-order: default
```

可选参数：

* default：按配置文件定义节点顺序
* latency：按节点延迟升序排列
* alphabet：按节点名称字母表排列

