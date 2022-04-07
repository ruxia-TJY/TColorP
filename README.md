# TColorP

[![](https://img.shields.io/badge/language-Python-blue)](https://www.python.org/) ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/ruxia-TJY/TColorP) ![linux](https://img.shields.io/badge/-Linux-yellow?logo=linux) ![windows](https://img.shields.io/badge/-Windows-blue?logo=windows)

print with color.

```python
from TColorP import TColorP, TColor

tcp = TColorP()
tcp.success('success')
tcp.error('error')
tcp.warning('warning')
tcp.normal('normal')

tcp.formatColor([TColor.method_normal, TColor.foreground_cyan])
print('hello')
tcp.formatColor([TColor.method_normal])
print('TColorP')
```

![view](View.png)

## how to use
```python
from TColorP import TColorP, TColor

tcp = TColorP()

# print success info 
tcp.success('success')
# print error info
tcp.error('error')
# print warning info
tcp.warning('warning')
# print normal info
tcp.normal('normal')

# print normal Style
print(tcp.normalStyle)

# change normal style
tcp.normalStyle = [TColor.method_highlight,TColor.foreground_red]
tcp.normal("normal")

# change normal style once
tcp.normal('normal once',style=[TColor.method_highlight,TColor.foreground_red])

# format color
tcp.formatColor([TColor.method_normal,TColor.foreground_red])
print('this will change color with red')

# print suppos method and color
print(TColor())
# method_normal=0,method_highlight=1,method_underline=4,method_reverse=7
# foreground_black=30,foreground_red=31,foreground_green=32,foreground_yellow=33,foreground_blue=34,foreground_fuchsia=35,foreground_cyan=36,foreground_white=37
# background_black=40,background_red=41,background_green=42,background_yellow=43,background_blue=44,background_fuchsia=45,background_cyan=46,background_white=47
```

## License

MIT License,Thanks!