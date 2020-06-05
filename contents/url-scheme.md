# URL Scheme

## 下载配置 <a id="&#x4E0B;&#x8F7D;&#x914D;&#x7F6E;"></a>

CFW支持使用URL Scheme快速导入配置文件：

```text
clash://install-config?url=
```

### 自定义名称 <a id="&#x81EA;&#x5B9A;&#x4E49;&#x540D;&#x79F0;"></a>

在CFW中使用URL导入后显示的配置文件名称识别逻辑如下：

1. 响应体头部中是否存在`content-disposition`字段，如果存在则使用里面`filename`对应的值
2. 使用URL最后一部分作为配置文件名

## 退出软件 <a id="&#x9000;&#x51FA;&#x8F6F;&#x4EF6;"></a>

```text
clash://quit
```

