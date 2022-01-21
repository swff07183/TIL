## 코드 스타일 가이드

- 파이썬에서 제안하는 스타일 가이드
  - [PEP8](https://www.python.org/dev/peps/pep-0008/)

- 기업, 오픈소스 등에서 사용되는 스타일 가이드
  - [Google Style guide](https://google.github.io/styleguide/pyguide.html)



## json 파일 불러오기

```python
import json

FILE_DIR = "data/a.json"

file_json = open(FILE_DIR, encoding='UTF8')
file_data = json.load(file_json)
```

