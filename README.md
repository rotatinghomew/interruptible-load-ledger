# 园区减载接棒与实绩清分

园区企业交换人工作业窗口和总表计量，用于登记可中断用电承诺和账务核对。资料中的工厂、读数与合同均为合成。

业务记录使用 [《厂区计量和响应单据》](docs/exchange.md) 的格式。`data/` 中含各参与方合成单据，可由 Python 3.11.2 读取，无需第三方包。SQLite 来自 Python 自带模块。

## 交换资料

在项目根目录启动本地资料源，可按 JSON 文件名访问记录。

```sh
python3 -m http.server --bind 127.0.0.1 --directory data 8411
```

## 资料校验

```sh
python3 -m unittest discover -s tests -v
```
