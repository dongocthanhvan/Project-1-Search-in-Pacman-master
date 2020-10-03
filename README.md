# CS188x_1-Artificial-Intelligence-Berkeley
Project solutions for CS188 Artificial Intelligence course

Question 1 (3 points): Finding a Fixed Food Dot using Depth First Search
Trong bài tập này ta dùng stack- hoạt động theo nguyên lý LIFO (Last in First out). Đưa điểm bắt đầu vào Stack .Nếu trạng thái được duyệt qua thì ta bỏ qua trạng thái này duyệt trạng thái tiếp theo, nếu chưa được duyệt qua thì thêm trạng thái vào visited. Nếu Stack rỗng, tìm kiếm kết thúc. Từ quá trình chạy cho đến khi về đích, ta đều lưu các action của từng state trong stack. Khi về đích( trạng thái kết thúc), sẽ trả về tất cả hành động dẫn đến trạng thái đó và kết thúc. Nếu chưa kết thúc, ta dùng hàm getSuccessors để tìm trạng tháitiếp theo rồi đưa vào stack tiếp theo.Ngoài ra ta còn tạo ra 1 list khác để lưu các vị trí đã được duyệt.

Question 2 (3 points): Breadth First Search
 Trong bài tập này ta dùng Queue - hoạt động theo nguyên lý FIFO (First in First out). Đưa điểm bắt đầu vào Queue. Nếu trạng thái được duyệt qua thì ta bỏ qua trạng thái này, nếu chưa được duyệt qua thì thêm trạng thái vào visited .Nếu queue rỗng, tìm kiếm kết thúc. Từ quá trình chạy cho đến khi về đích, ta đều lưu các action của từng state trong queue. Khi về đích( trạng thái kết thúc), sẽ trả về tất cả hành động dẫn đến trạng thái đó và kết thúc. Nếu chưa kết thúc, ta dùng hàm getSuccessors để tìm trạng thái tiếp theo rồi đưa vào queue tiếp theo.Ngoài ra ta còn tạo ra 1 list khác để lưu các vị trí đã được duyệt.
 
Question 3 (3 points): Varying the Cost Function
Tương tự câu 1, 2 nhưng sẽ dùng Priority Queue và có thêm  độ ưu tiên được xác định bằng tổng giá trị các bước để về đích, ưu tiên sẽ được xếp đầu hàng đợi nếu tổng giá trị nhỏ hơn. Nếu Priority Queue rỗng, tìm kiếm kết thúc. Đưa điểm bắt đầu vào Queue. Nếu trạng thái được duyệt qua thì ta bỏ qua trạng thái này, nếu chưa được duyệt qua thì thêm trạng thái vào visited. Khi về đích( trạng thái kết thúc), sẽ trả về tất cả hành động dẫn đến trạng thái đó và kết thúc. Nếu chưa kết thúc, ta dùng hàm getSuccessors để tìm trạng thái tiếp theo rồi đưa vào queue tiếp theo.

Question 4 (3 points): A* search
Tương tự uniformCostSearch nhưng thêm heuristic là khoảng cách từ điểm đó đến đích, khoảng cách ngắn hơn thì được ưu tiên lên đầu hàng đợi. Điểm bắt đầu tại PriorityQueue . Nếu PriorityQueue rỗng kết thúc tìm kiếm. Khi về đích( trạng thái kết thúc), sẽ trả về tất cả hành động dẫn đến trạng thái đó và kết thúc. Nếu chưa kết thúc, ta dùng hàm getSuccessors để tìm trạng thái tiếp theo rồi đưa vào queue tiếp theo.