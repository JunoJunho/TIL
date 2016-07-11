# Read xlsx file

R에서 여러가지 파일을 읽어서 데이터를 처리합니다. xlsx 파일을 읽기 위하여는 다음의 코드 조각이 필요합니다.

```
library(xlsx) # 없는 경우 install.packages('xlsx')

data <- read.xlsx(file_directory_and_name, sheetIndex = 1) # 1 번째 시트에 있는 내용 읽어오기
data <- read.xlsx(file_directory_and_name, sheetName = 'n1')
```
