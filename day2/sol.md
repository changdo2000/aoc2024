# https://adventofcode.com/2024/day/2

## Tóm tắt đề 

### Bài 1

Cho N dãy số. Đếm số dãy số thỏa mãn các điều kiện sau:

1. Dãy số là dãy số tăng hoặc là dãy số giảm.

2. Hai số đứng cạnh nhau ít hơn 3.

VD: 

    7 6 4 2 1: Thỏa mãn vì các cấp độ đều giảm đi 1 hoặc 2.
    1 2 7 8 9: Không thỏa mãn vì 2 7 là tăng 5.
    9 7 6 2 1: Không thỏa mãn vì 6 2 là số giảm của 4.
    1 3 2 4 5: Không thỏa mãn vì 1 3 tăng nhưng 3 2 giảm.
    8 6 4 4 1: Không thỏa mãn vì 4 4 không tăng cũng không giảm.
    1 3 6 7 9: Thỏa mãn vì các cấp độ đều tăng dần 1, 2 hoặc 3.

### Bài 2

Các điều kiện giữ nguyên như bài 1.

Dãy được tính khi thỏa mãn các điều kiện trên hoặc bỏ một số bất kỳ để tạo ra dãy thỏa mãn

## Cách làm

### Bài 1

=> Kiểm tra dãy có phải dãy tăng / giảm và tính chênh lệnh giữa 2 số liên tiếp trong dãy.

### Bài 2

=> Duyệt tất cả các vị trí trong dãy, bỏ số ở vị trí đó ra và check xem dãy có thỏa mãn điều kiện hay không.
