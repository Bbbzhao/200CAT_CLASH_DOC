# 启动第三方应用

## 启动其他应用 <a id="&#x542F;&#x52A8;&#x5176;&#x4ED6;&#x5E94;&#x7528;"></a>

版本0.6.1更新后，加入启动其他第三方应用的能力。可以在CFW启动后自动启动其他软件

## 使用 <a id="&#x4F7F;&#x7528;"></a>

在`Home Directory`目录中`config.yaml`文件中加入如下配置：

```text
cfw-child-process:
  - command: bark-helper-go.exe  # 程序名称
    args:
      - "-t" # 运行参数1
      - "abcdefghijk" # 运行参数2
    options:
      cwd: C:\bark-helper # 子进程工作目录
```

添加完毕后重启CFW即可生效

其他参数参考：[http://nodejs.cn/api/child\_process.html\#child\_process\_child\_process\_spawn\_command\_args\_options](http://nodejs.cn/api/child_process.html#child_process_child_process_spawn_command_args_options)

