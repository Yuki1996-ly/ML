Fine-tuning vs Prompting  对于大型语言模型的两种不同期待

1.1GPT是文字接龙，Bert是文字填空

<img src="C:\Users\admin\Documents\GitHub\ML\Photoes\image-20230713164459207.png" alt="image-20230713164459207" style="zoom:25%;" />

1.2.1 我们对于语言模型的期待，通常有两种，一种是让其成为专才，一种是让其成为通才。在成为专才的情况下比如Bert，由于其本身做的是做完形填空的方式，所以对于像翻译这样的要求是没有办法完成的，所以我们需要外挂，比如Fine-tuning，fine-tuning是利用原来的语言参数作为初始化的参数，对其进行几次梯度训练gradient descent。以达到专才的效果.

1.2.2第二种技术是大模型本身是不动的，加入adapter，应该是插件的意思，在adapter上去进行微调，这样可以达到fine-tune的效果，成为专才。

<img src="C:\Users\admin\Documents\GitHub\ML\Photoes\image-20230713165800328.png" alt="image-20230713165800328" style="zoom:25%;" />



2.对于In-context Learning来说，模型越大，会受到文本影响的概率就越大

<img src="C:\Users\admin\Documents\GitHub\ML\Photoes\image-20230713172258560.png" alt="image-20230713172258560" style="zoom:25%;" />

2.2 Flan是有训练过通过人类的指令来做训练的，所以效果会比GPT3没有in-context learning 和few-context learning效果要好

<img src="C:\Users\admin\Documents\GitHub\ML\Photoes\image-20230713173029411.png" alt="image-20230713173029411" style="zoom:25%;" />