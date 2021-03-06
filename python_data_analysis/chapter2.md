### 可实现的功能

- 与外界进行交互

读写各种各样的文件格式与数据库

- 准备

对数据进行清理、修整、整合、规范化、重塑、切片切块、变形等处理以便进行法分析。

- 转换

对数据集做一下数学和统计运算以产生新的数据集。比如说，根据分组变量对一个大表进行聚合。

- 建模与计算

将数据跟统计模型、机器学习算法或其他计算工具联系起来。

- 展示

创建交互式的或静态的图片或文字摘要。

### 一些代码

- 列表推导式（list comprehension）

在一组字符串（或一组别的对象）上执行一条相同操作

eg.records = [json.loads(line) for line in open(path)]

- 计数

```
def get_counts(sequence):
    counts = {}
    for x in sequence:
        if x in counts:
            counts[x] += 1
        else:
            counts[x] = 1
    return counts
```

利用python标准库

```
from collections import defaultdict

def get_counts2(sequence):
    counts = defaultdict(int) # 所有的值均会被初始化为0
    for x in sequence:
        counts[x] += 1
    return counts
```

### little tips

python 的索引是从0开始的，R语言的索引是从1开始的。

