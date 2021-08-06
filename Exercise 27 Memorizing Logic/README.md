# The Truth Terms
Trong python chúng ta có các thuật ngữ như sau (Ký tự hoặc là mệnh đề) để xác định xem điều gì "Đúng" hoặc "Sai". Logic trên máy tính xem xét tất cả xem liệu sự kết hợp của các mệnh đề này và một số giá trị True tại thời điểm đó trong chương trình.
* and 
* or 
* not 
* != (không bằng)
* == (bằng)
* \>= (lớn hơn hoặc bằng)
* <= (bé hơn hoặc bằng)
* True
* False
# The Truth Table
Bây giờ chúng ta sẽ sử dụng các mệnh đề này để lập bảng chân trị (The Truth Table) mà bạn cần ghi nhớ.

|NOT|True?|
|---|-----|
|not False|True|
|not True|False|

|OR| True?|
|---|-----|
|True or False| True|
|True or True| True|
|False or True| True|
|False or False| False|

|AND| True?|
|----|-----|
|True and False| False|
|True and True| True|
|False and True| False|
|False and False| False|

|NOT OR| True?|
|-----|------|
|not (True or False)| False|
|not (True or True)| False|
|not (False or True)| False|
|not (False or False)| True|

|NOT AND| True?|
|----|---|
|not (True and False)| True|
|not (True and True)| False|
|not (False and True)| True|
|not (False and False)| True|

|!=| True?|
|---|--|
|1 != 0| True|
|1 != 1| False|
|0 != 1 |True|
|0 != 0 |False|

|==| True?|
|---|----|
|1 == 0| False|
|1 == 1 |True|
|0 == 1 |False|
|0 == 0 |True|

