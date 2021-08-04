Khác với các bài trước, ở bài này mình sẽ thực thi từng hàm ở file ex25.py trong **trình biên dịch python(python3 interpreter)**.
# WHAT YOU SHOULD SEE
Mình sẽ khởi động python3 interpreter trước. Bạn sẽ thấy nó sẽ có giao diện như thế này.
![image](https://user-images.githubusercontent.com/83932775/128228341-3c93261f-7198-4bb4-b8ac-842049709c9c.png)
Sau dấu nhắc lệnh "<" (hay còn gọi là prompt) bạn có thể gõ code Python vào đó và nó sẽ được thực thi ngay lập tức. Bằng cách này chúng ta có thể gõ từng dòng Python code như bên dưới và xem chúng làm gì:
```
import ex25
sentence = "All good things come to those who wait."
words = ex25.break_words(sentence)
words
sorted_words = ex25.sort_words(words)
sorted_words
ex25.print_first_word(words)
ex25.print_last_word(words)
words
ex25.print_first_word(sorted_words)
ex25.print_last_word(sorted_words)
sorted_words
sorted_words = ex25.sort_sentence(sentence)
sorted_words
ex25.print_first_and_last(sentence)
ex25.print_first_and_last_sorted(sentence)
```
Kết quả sẽ giống như thế này khi bạn nhập từng dòng ở trên:
```
Python 3.9.0 (tags/v3.9.0:9cf6752, Oct  5 2020, 15:34:40) [MSC v.1927 64 bit (AMD64)] on win32Type "help", "copyright", "credits" or "license" for more information.
>>> import ex25
>>> sentence = "All good things come to those who wait."
>>> words = ex25.break_words(sentence)
>>> words
['All', 'good', 'things', 'come', 'to', 'those', 'who', 'wait.']
>>> sorted_words = ex25.sort_words(words)
>>> sorted_words
['All', 'come', 'good', 'things', 'those', 'to', 'wait.', 'who']
>>> ex25.print_first_word(words)
All 
>>> ex25.print_last_word(words)
wait.
>>> words
['good', 'things', 'come', 'to', 'those', 'who']
>>> ex25.print_first_word(sorted_words) 
All
>>> ex25.print_last_word(sorted_words)
who
>>> sorted_words
['come', 'good', 'things', 'those', 'to', 'wait.']
>>> sorted_words = ex25.sort_sentence(sentence)
>>> sorted_words
['All', 'come', 'good', 'things', 'those', 'to', 'wait.', 'who']
>>> ex25.print_first_and_last(sentence)
All
wait.
>>> ex25.print_first_and_last_sorted(sentence)
All
who                                         
```
Khi bạn xem qua từng dòng này, hãy đảm bảo rằng bạn có thể tìm thấy các hàm này được chạy trong ex25.py và hiểu cách hoạt động của chúng. Nếu bạn nhận về một kết quả khác hoặc lỗi, bạn sẽ phải tự sữa lại code của mình, sau đó thử lại một lần nữa.
# Common Student Questions
- **Nhận được giá trị "None"** .Thử kiểm tra lại các hàm xem bạn đã dòng return ở cuối mỗi hàm chưa.
- **-bash: import: command not found khi chạy import ex25**. Đảm bảo bạn chạy các lệnh trong python3 interpreter không phải trong terminal.
- **ImportError: No module named ex25.py**. Hãy gõ import ex25 thay vì import ex25.py. Bạn không cần phải thêm .py, python mặc định biết điều đó với file extension .py.
- **SyntaxError: invalid syntax**. Sai lỗi cú pháp ví dụ như thiếu ( hoặc ".
