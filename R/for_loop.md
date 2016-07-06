# For loop in R

R에서 반복문을 사용하는 방법

Python, Ruby 등과 같이 다른 스크립트에서 있는 for each 구문은 R에서는 존재하지 않습니다. 대신 length를 사용하여 작성합니다.

```
for(a in 1:50){
  print(a) # Expected output: 1 to 50
}

# or

for(i in 1:length(list_l)){
  print(list_l[i]) # print each item in list_i
}

```
