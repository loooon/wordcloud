# wordcloud


- This is a simple project to generate wordcloud via python.


> Q:`How to use?`

+ A:
```
pip install wordcloud


```

```
参数
类型
描述
font_path 
string 
指定字体的位置(可以在网上下载OTF或者TTF格式),默认使用DroidSansMono path 
width 
int(default=400) 
图片宽度，越大越精细 
height 
int (default=200) 
图片高度，越大越精细 
prefer_horizontal 
float (default=0.90) 
越接近1说明越喜欢水平的字，则字就不会为了适合展示而翻转成水平的 
mask : nd-array or None (default=None) 
将词云画在遮罩上 
scale : float (default=1) 
计算和画图的比例，当做大图的时候使用scale代替height和width速度会快，但会影响词之间的拟合度 
min_font_size : int (default=4) 
最小频率词的大小 
font_step : int (default=1) 
字体步长，如果大于1，可以增快计算速度，但是拟合度会下降 
max_words : number (default=200) 
图片容纳词语的上限 
stopwords : set of strings or None 
设置停用词，如果不设置则使用默认的停用词 
background_color : color value (default=”black”) 
背景颜色设置 
max_font_size : int or None (default=None) 
最大的词语的大小 
mode : string (default=”RGB”) 
当使用”RGBA”时，背景将变成透明的 
relative_scaling : float (default=.5) 
当relative_scaling=0时，词的大小是按照排名计算的，当relative_scaling=1时候则会按词频的倍数计算大小。 
color_func : callable, default=None 
根据每个词的font_size, position, orientation, font_path, random_state等属性为词语生成特定的颜色，具体参考matplotlib colormap 
regexp : string or None (optional) 
collocations : bool, default=True 
是否考虑词语的搭配 
colormap : string or matplotlib colormap, default=”viridis” 
Matplotlib colormap，如果color_func参数被指定，则此参数无效 
normalize_plurals : bool, default=True 
是否忽略复数 
属性
类型
描述
words_ 
(dict of string to float) 
返回词频 
layout_ 
(list of tuples (string, int, (int, int), int, color))) 
词云词的属性信息 
方法
描述
fit_words(frequencies) 
元组形式(word,freq) 
generate(text) 
文本形式 
generate_from_frequencies(frequencies[, …]) 
字典形式{word:freq} 
generate_from_text(text) 
process_text(text) 
分割文本，去除停用词 
recolor([random_state, color_func, colormap]) 
重新对图层上色 
to_array() 
to_file(filename) 
to_html() 
to_image() 
```
