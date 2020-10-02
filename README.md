# Berkeley_search

# Bài 1 đến bài 4: cài theo thuật toán được dạy trên lớp

DFS dùng stack

BFS dùng queue

UCS dùng priority queue với cost

A* dùng priority queue với total dist + cost + heuristic

# Bài 5:
Thêm 1 biến để lưu những góc chưa đi qua

Kết thúc khi biến remainCornor có len = 0

# Bài 6:
Nếu tính heuristic là khoảng cách manhantta nhỏ nhất đến 1 góc và cộng thêm số lượng góc còn lại, số node tầm khoảng 1400, không tối ưu. Brute force, tính tổng mọi khoảng cách manhattan với tất cả cách sắp xếp các cornor còn lại sau khi bỏ đi 1 góc, lấy giá trị nhỏ nhất làm heuristic, chương trình thu gọn lại còn khoảng 770 node

# Bài 7:
Đã thử làm theo 3 cách: khoảng cách manhatta nhỏ nhất + số thức ăn còn lại - 1, cần khoảng 11k node, không tối ưu.

Sử dụng thêm bao lồi và tính tổng khoảng cách đi qua các điểm trên bao lồi khi sô điểm > 5, vẫn cần hơn 9k node, tốt hơn nhưng chưa đủ. Dưới 5 điểm,có thể do lỗi cài đặt hoặc ý tưởng sai, heuristic đều dài hơn con đường thực tế.

Thử lấy khoảng cách ngắn nhất đến food và khoảng cách dài nhất giữa 2 food, cần 7k7 node, đủ tối ưu để max điểm, nhưng chưa lấy được extra credit ;-;

# Bài 8:
Kiểm tra đích : khi vị trí của pacman năm trong food list của trò chơi

Tìm kiếm : BFS chạy và max điểm, DFS chưa test
