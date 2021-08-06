Các sự kết hợp logic mà bạn đã học được từ bài tập trước được gọi là biểu thức Boolean. Biểu thức boolean được sử dụng rất nhiều trong lập trình. 

Trong bài tập này, bạn sẽ thực hiện các bài tập logic mà bạn đã ghi nhớ và bắt đầu thử chúng bằng Python. Trong mỗi trường hợp, kết quả sẽ là Đúng hay sai. Khi bạn đã viết ra câu trả lời, hãy bắt đầu Python trong Terminal của bạn và nhập từng vấn đề logic để xác nhận câu trả lời của bạn. 

1. True and True
2. False and True
3. 1 == 1 and 2 == 1
4. "test" == "test"
5. 1 == 1 or 2 != 1
6. True and 1 == 1
7. False and 0 != 0
8. True or 1 == 1
9. "test" == "testing"
10. 1 != 0 and 2 == 1
11. "test" != "testing"
12. "test" == 1
13. not (True and False)
14. not (1 == 1 and 0 != 1)
15. not (10 == 1 or 1000 == 1000)
16. not (1 != 10 or 3 == 4)
17. not ("testing" == "testing" and "Zed" == "Cool Guy")
18. 1 == 1 and (not ("testing" == 1 or 1 == 0))
19. "chunky" == "bacon" and (not (3 == 4 or 3 == 3))
20. 3 == 3 and (not ("testing" == "testing" or "Python" == "Fun"))

Tôi cũng sẽ cung cấp cho bạn một mẹo để giúp bạn tìm ra đáp án ở những cái phức tạp hơn về cuối.
Bất cứ khi nào bạn nhìn thấy các mệnh đề logic Boolean này, bạn có thể giải quyết chúng một cách dễ dàng bằng quy trình đơn giản sau:
1. Tìm một mệnh đề kiểm tra bằng nhau (== hoặc! =) Và thay thế nó bằng chân trị của nó.
2. Tìm mỗi mệnh đề and/or bên trong dấu ngoặc đơn và giải quyết chúng trước.
3. Tìm từng cái not và đảo ngược giá trị nó.
4. Tìm bất kỳ mệnh đề còn lại của  and/or và giải quyết nó.
5. Khi bạn làm xong, bạn sẽ có  kết quả True hoặc False.

Tôi sẽ lấy ví về cách áp dụng trick này ở trường hợp số 20:

3 != 4 and not ("testing" != "test" or "Python" == "Python")

Sau đây là tôi đi qua từng bước và hiển thị cho bạn cách làm chi tiết cho đến khi tôi nhận được kết quả duy nhất:

1. Giải các mệnh đề bằng nhau:
3 != 4 is True: True and not ("testing" != "test" or "Python" == "Python")
"testing" != "test" is True: True and not (True or "Python" == "Python")
"Python" == "Python": True and not (True or True)
2. Tìm and / or trong dấu ngoặc đơn ()
(True or True) is True: True and not (True)
3. Tìm mệnh đề not và đảo ngược giá trị của nó
not (True) is False: True and False
4. Tìm các mệnh đề and/or còn lại:
True and False is False
Với việc hoàn thành các bước trên chúng ta thu được kết quả của biểu thức là False.
# What would you see
Sau khi bạn cố gắng đoán các kết quả từ các mệnh đề, chúng ta có thể kiểm la lại với Python như thế này:
![image](https://user-images.githubusercontent.com/83932775/128553254-f70fdb01-038e-4c75-9ccc-5588eaf69397.png)
# Common Student Questions
**Tại sao "test" and "test" trả về giá trị "test" hoặc 1 or 1 trả về giá trị 1 thay vì chúng trả về giá trị True?** Python và nhiều ngôn ngữ khác sẽ trả về một trong các toán hạng trong toán tử Boolean của chúng hơn là chỉ trả về giá trị True hoặc False. Điều này có nghĩa là nếu bạn lấy True and 1 bạn sẽ nhận được kết quả trả về là toán hạng đầu tiên (False), nhứng nếu bạn lấy True and 1 thì bạn sẽ nhận được kết quả trả về là toán hạng thứ 2 (1).

**Có bất kỳ điểm khác biệt nào giữa != và <>?** Python đã không dùng <> nữa vì vậy hãy dùng !=. Ngoài ra không có sự khác biệt về ý nghĩa.

# My solution
|STT|Logic problem|Result|
|---|----|----|
|1| True and True|True|
|2| False and True|False|
|3| 1 == 1 and 2 == 1|False|
|4| "test" == "test"|True|
|5| 1 == 1 or 2 != 1|True|
|6| True and 1 == 1|True|
|7| False and 0 != 0|False|
|8| True or 1 == 1|True|
|9| "test" == "testing"|False|
|10| 1 != 0 and 2 == 1|False|
|11| "test" != "testing"|True|
|12| "test" == 1|False|
|13| not (True and False)|True|
|14| not (1 == 1 and 0 != 1)|False|
|15| not (10 == 1 or 1000 == 1000)|False|
|16| not (1 != 10 or 3 == 4)|False|
|17| not ("testing" == "testing" and "Zed" == "Cool Guy")|True|
|18| 1 == 1 and (not ("testing" == 1 or 1 == 0))|True|
|19| "chunky" == "bacon" and (not (3 == 4 or 3 == 3))|False|
|20| 3 == 3 and (not ("testing" == "testing" or "Python" == "Fun"))|False|
