# 打断连接

默认情况下，CFW不会在任何时候主动打断正在进行的连接（Connections），连接会被保持到主动断开。

如果在特定情况下，需要在切换节点后或切换配置文件前先打断连接，可以在[General YAML](ui/chang-gui-general.md)中进行如下配置：

```text
cfw-conn-break-strategy:
  proxy: none              # none/chain/all
  profile: true            # true/false
  mode: false              # true/false
```

## 选项说明 <a id="&#x9009;&#x9879;&#x8BF4;&#x660E;"></a>

### proxy <a id="proxy"></a>

* none：默认值，不进行打断
* chain：打断所有chains中包含此策略组的连接
* all：打断所有连接

### profile <a id="profile"></a>

* true：切换配置前先打断所有连接
* false：不打断

### mode <a id="mode"></a>

* true：切换代理模式（Direct/Rule/Global）时断开所有连接
* false：不打断

