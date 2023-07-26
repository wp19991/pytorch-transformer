# pytorch-transformer

```bash
conda create -n pytorch2 python=3.10
conda activate pytorch2
conda install pytorch torchvision torchaudio torchtext pytorch-cuda=11.8 -c pytorch -c nvidia
pip install portalocker>=2.0.0

# 安装分词器
pip install spacy
# 下载地址：https://github.com/explosion/spacy-models/
pip install de_core_news_sm-3.6.0-py3-none-any.whl
pip install en_core_web_sm-3.6.0-py3-none-any.whl
```

```
pytorch复现transformer

数据集: 德语翻译英语
```

# 运行效果

```
$ python evaluation.py
Zwei junge weiße Männer sind im Freien in der Nähe vieler Büsche. -> Two young , White males are outside near many bushes .
Mehrere Männer mit Schutzhelmen bedienen ein Antriebsradsystem. -> Several men in hard hats are operating a giant pulley system .
Ein kleines Mädchen klettert in ein Spielhaus aus Holz. -> A little girl climbing into a wooden playhouse .
Ein Mann in einem blauen Hemd steht auf einer Leiter und putzt ein Fenster. -> A man in a blue shirt is standing on a ladder cleaning a window .
Zwei Männer stehen am Herd und bereiten Essen zu. -> Two men are at the stove preparing food .
Ein Mann in grün hält eine Gitarre, während der andere Mann sein Hemd ansieht. -> A man in green holds a guitar while the other man observes his shirt .
Ein Mann lächelt einen ausgestopften Löwen an. -> A man is smiling at a stuffed lion
Ein schickes Mädchen spricht mit dem Handy während sie langsam die Straße entlangschwebt. -> A trendy girl talking on her cellphone while gliding slowly down the street .
```

# 说明

```
ref: 理论
checkpoints: 训练好的model
train.py：训练
evaluation.py：预测
```