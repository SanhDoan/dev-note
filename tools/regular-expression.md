- `[xyz]` Tìm và so sánh với tất cả các kí tự trong dấu ngoặc vuông và trùng khớp với 1 kí tự trong dấu ngoặc vuông
- `[a-z]` So sánh và trùng khớp với một ký tự nằm trong khoảng chỉ định
- `[^xyz]` So sánh và không trùng khớp với những ký tự nằm trong khoảng chỉ định. Dấu `^` (dấu mũ) nằm trong dấu ngoặc vuông là một dấu phủ định
- `^` Trùng khớp với phần đầu của chuỗi đích. Ví dụ: `^a` sẽ trùng khớp với chữ a trong chuỗi <strong>abc</strong>
- `$` Trùng khớp với phần cuối của chuỗi đích. Ví dụ: `c$` sẽ trùng khớp với chữ c trong chuỗi <strong>abc</strong>
- `+` Trùng khớp với 1 hoặc nhiều lần ký tự đứng trước nó. Ví dụ `\d+` sẽ chỉ trùng với chuỗi có từ 1 con số trở lên
- `*` Trùng khớp với 0 hoặc nhiều lần ký tự đứng trước nó. Ví dụ `\d*` sẽ trùng với chuỗi có chứa 1 chữ số hoặc không có chữ số nào cũng được
- `?` Trùng khớp với 0 hoặc 1 lần ký tự đứng trước nó
- `.` Trùng khớp với 1 ký tự đơn bất kỳ ngoại trừ ký tự ngắt dòng (line-break) và cũng không lấy được ký tự có dấu (unicode)
- `x{n}` Trùng khớp đúng với n lần ký tự đứng trước nó. n là một số không âm. Ví dụ `\d{2}` sẽ bắt đc các số có 2 chữ số đứng liền nhau
- `x{n,}` Trùng khớp với ít nhất n lần ký tự đứng trước nó. n là một số không âm
- `x{n,m}` Trùng khớp với ít nhất n lần và nhiều nhất là m lần ký tự đứng trước nó
- `x|y` Trùng khớp với x hoặc y
- `\b` Trùng khớp với toàn bộ ký tự đứng trước nó
- `\B` Ngược lại với `\b`, `\B` sẽ không khớp với toàn bộ mà chỉ 1 phần ký tự đứng trước nó
- `\d` Trùng khớp 1 ký tự số (digit)
- `\D` Trùng khớp 1ký tự không phải số (non-digit)
- `\s` Trùng khớp 1 ký tự khoảng trắng (whitespace) bao gồm khoảng trắng tạo ra bởi phím Tab
- `\S` Trùng khớp với 1 ký tự không phải là khoảng trắng (non-whitespace)
- `\w` Trùng khớp với các ký tự là từ (word) bao gồm dấu _ (underscore) và chữ số
- `\W` Trùng khớp với các ký tự không phải là từ (non-word). Ví dụ: `\W` sẽ khớp với ký tự `%` trong chuỗi "100%"
- `\uxxxx` Trùng khớp với 1 ký tự unicode. Ví dụ: `\u00FA` sẽ khớp với ký tự "ú", `\u00F9` sẽ khớp với ký tự "ù"
- `\pL` Trùng khớp với một ký tự Unicode bất kỳ ngoại trừ dấu cách. Đây chính là cú pháp viết hoàn hảo hơn của dấu `.`,Ví dụ `\pL+` sẽ lấy được chuỗi `truyền, thuyết` trong chuỗi <strong>"truyền thuyết"</strong>

Tham khảo: https://viblo.asia/p/hoc-regular-expression-va-cuoc-doi-ban-se-bot-kho-updated-v22-Az45bnoO5xY