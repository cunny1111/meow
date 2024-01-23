***Những phần nào đánh dấu * là những phần nên biết. List bao gồm các link diễn giải chi tiết về các chủ đề có trong cấu trúc đề thi chọn học sinh giỏi cấp tỉnh THPT, một số bao gồm thêm các bình luận về chủ đề.***

***==Listed by Zawajiro / Vu Huy Cuong==***

##### ***`Thuật toán số học`***

> **Số nguyên tố:**
> https://jmp.sh/s/hUJMbLhkTDrbqIMYLDcH
1. * Sieve of Eratosthenes (Sàng số nguyên tố Eratosthenes)
   - Dùng để liệt kê các số nguyên tố một cách tối ưu
   - Không hiệu quả để kiểm tra xem một số có phải số nguyên tố hay không
   - https://vnoi.info/wiki/translate/he/Number-Theory-2.md
2. Sieve of Atkin (Sàng số nguyên tố Atkin)
   - Sàng Eratosthenes nhưng phức tạp và chạy nhanh hơn
   - Nên sử dụng nếu bài toán yêu cầu các số rất lớn (lên tới 10^12 trở lên)
   - Khá khó để áp dụng vì độ phức tạp của thuật toán cao
   - Ý tưởng của thuật toán:
     - *Tất cả các số dư là [số dư](https://vi.wikipedia.org/wiki/S%E1%BB%91_d%C6%B0 "Số dư") khi [chia](https://vi.wikipedia.org/wiki/Ph%C3%A9p_chia "Phép chia") cho 60 (chia cho 60 và xét số dư).*
     - *Tất cả các số, bao gồm cả x và y đều là [số nguyên](https://vi.wikipedia.org/wiki/S%E1%BB%91_nguy%C3%AAn "Số nguyên") dương.*
     - *Đảo một ô trong sàng nghĩa là thay đổi đánh dấu (là [số nguyên tố](https://vi.wikipedia.org/wiki/S%E1%BB%91_nguy%C3%AAn_t%E1%BB%91 "Số nguyên tố") hoặc không) thành ngược lại.*
       1. *Tạo bảng kết quả, điền vào 2, 3, và 5.*
       2. *Tạo bảng sàng nguyên tố với các số nguyên dương; tất cả các số đánh dấu là không nguyên tố.*
       3. *Với tất cả các số trong sàng:*
          - *Nếu số đó chia 60 dư 1, 13, 17, 29, 37, 41, 49, hoặc 53, đảo đánh dấu cho các số ở $4 * x^2 + y^2 =$ số đang xét.*
          - *Nếu số đó chia 60 dư 7, 19, 31, hoặc 43, đảo các ô $3 * x^2 + y^2 =$ số đang xét.*
          - *Nếu số đó chia 60 dư 11, 23, 47, hoặc 59, đảo các số $3 * x^2 - y^2 =$ số đang xét.*
          - *Nếu không, không làm gì cả*
       4. *Bắt đầu từ số nhỏ nhất trong sàng.*
       5. *Lấy các số tiếp theo trong sàng được đánh dấu là prime.*
       6. *Thêm vào danh sách kết quả.*
       7. *Bình phương số đó và đánh dấu các bội số của số đó là không phải số nguyên tố.*
       8. *Lặp lại bước 5 cho tới bước 8.*
   - https://vi.wikipedia.org/wiki/Sàng_Atkin
   - https://www.geeksforgeeks.org/sieve-of-atkin/ 
3. * Primality Test (Kiểm tra nguyên tố)
   - https://vnoi.info/wiki/algo/algebra/primality_check.md

> **Tính chẵn lẻ:**
> https://gochocit.com/ky-thuat-lap-trinh/kiem-tra-so-chan-le-trong-c

> * **Số chính phương:**
> https://codehow.net/thuat-toan-kiem-tra-so-chinh-phuong-trong-c-c++-72.html
> https://freetuts.net/thuat-toan-kiem-tra-so-chinh-phuong-2921.html

> **Số bậc thang:**
> https://hoidap247.com/cau-hoi/2586513

> **Fibonacci:**
> https://viettuts.vn/bai-tap-cpp/day-so-fibonacci-trong-cpp

##### ***`Thuật toán xâu`***

> **Thuật toán cơ bản:**
> https://vnoi.info/wiki/languages/cpp/string.md
1. Ghép chuỗi:
   - *Có thể sử dụng toán tử `+` hoặc `+=`.*
2. So sánh chuỗi:
   - *Có thể so sánh hai chuỗi theo thứ tự từ điển bằng `==`, `!=`, `>`, `>=`, `<`, `<=`.*
3. Truy cập từng ký tự:
   - *Sử dụng toán tử `[]` để truy cập từng ký tự của chuỗi.*
4. Độ dài chuỗi:
   - *Sử dụng hàm `length()` để lấy độ dài chuỗi.*

> **Thuật toán nâng cao:**
> https://vnoi.info/wiki/languages/cpp/string.md
> https://www.studocu.com/vn/document/hoc-vien-ngan-hang/nhap-mon-he-thong-thong-tin/chuyen-de-xau-hai-chuan-kien-thuc-nang-cao-ve-xau-cua-c/59540314
1. * Tìm kiếm chuỗi con:
   - *Sử dụng hàm `find()` để tìm vị trí đầu tiên của một chuỗi con trong chuỗi.*
   - *Sử dụng hàm `rfind()` để tìm từ phải qua trái*
2. Thay thế chuỗi con:
   - *Sử dụng hàm `replace()` để thay thế một chuỗi con bằng một chuỗi khác.*
3. Cắt chuỗi:
   - *Sử dụng hàm `substr()` để lấy một chuỗi con từ chuỗi.*
4. Đảo ngược chuỗi:
   - *Sử dụng hàm `reverse()` để đảo ngược chuỗi.*
5. * Chuyển đổi giữa chuỗi và số:
   - *Sử dụng hàm `atoi()` để chuyển từ chuỗi sang số.*
   - *Sử dụng hàm `to_string()` để chuyển từ số sang chuỗi.*
6. * Chèn & xóa chuỗi con:
   - *Sử dụng hàm `insert()` để chèn một chuỗi con vào một chuỗi.*
   - *Sử dụng hàm `erase()` để xóa một chuỗi con từ chuỗi.*

##### ***`Dữ liệu kiểu mảng`***

> **Min & Max:**
> https://laptrinhcanban.com/cpp/lap-trinh-cpp-co-ban/mang-trong-cpp/tim-max-va-min-trong-mang-cpp/
> https://blog.luyencode.net/tim-so-lon-nhat-trong-mang/

> **Sắp xếp:**
> https://codelearn.io/sharing/cac-thuat-toan-sap-xep-trong-cpp

> **Thuật toán tìm kiếm:**
> https://techacademy.edu.vn/cac-thuat-toan-tim-kiem-trong-c/
> https://topdev.vn/blog/thuat-toan-tim-kiem-trong-c/
> https://codelearn.io/sharing/5-thuat-toan-tim-kiem-moi-ltv-nen-biet

> **Kỹ thuật duyệt toàn bộ:**
> https://123docz.net/document/9216207-bai-tap-chuyen-de-duyet-toan-bo.htm

##### ***`Dữ liệu kiểu mảng 2`***

> **Truyền mảng vào hàm:**
> https://viettuts.vn/lap-trinh-cpp/truyen-mang-vao-ham-trong-cpp

> **Nhập và xuất mảng 1 chiều:**
> https://blog.luyencode.net/huong-dan-cach-nhap-mang-mot-chieu-trong-c/

> **Sao chép mảng 1 chiều:**
> https://laptrinhcanban.com/cpp/lap-trinh-cpp-co-ban/mang-trong-cpp/sao-chep-mang-trong-cpp/

> **Thêm và xóa phần tử trong mảng:**
> https://blog.28tech.com.vn/cpp-chen-va-xoa-phan-tu

##### ***`Thuật toán nâng cao`***

> * **Kỹ thuật 2 con trỏ:**
> https://storage-vnportal.vnpt.vn/lci-ubnd-responsive/sitefolders/thptchuyen-laocai/5258/chuyende/ki-thuat-2-con-tro.pdf

> **Kỹ thuật cộng dồn:**
> https://vnoi.info/wiki/algo/data-structures/prefix-sum-and-difference-array.md
> https://tek4.vn/khoa-hoc/cau-truc-du-lieu-va-thuat-toan/ky-thuat-mang-cong-don

##### ***`Thuật toán nâng cao 2`***

> * **Sắp xếp:**
> https://vnoi.info/wiki/algo/basic/sorting.md

> * **Tìm kiếm nhị phân:**
> https://vnoi.info/wiki/algo/basic/binary-search.md

> **STL (Standard Template Library):**
> https://zawajiro.tiiny.site

##### ***`Thuật toán, cấu trúc dữ liệu phức tạp: Thuật toán`***

> **Kỹ thuật duyệt:**
> https://cppdeveloper.com/c-nang-cao/cac-phuong-phap-duyet-qua-cac-phan-tu-cua-mot-container-trong-c/
> https://sinhvientot.net/duyet-mang-mot-chieu/

> **Nhánh cận:**
> https://viblo.asia/p/nhanh-va-can-branch-and-bound-Qbq5QBPEKD8

> **Đệ quy:**
> https://viettuts.vn/lap-trinh-cpp/de-quy-trong-cpp

> * **Chia để trị:**
> https://viblo.asia/p/chia-de-tri-divide-and-conquer-bJzKmd3r59N
> https://viblo.asia/p/tim-hieu-thuat-toan-chia-de-tri-va-cac-vi-du-ap-dung-3Q75wkP95Wb

> * **Quy hoạch động:**
> https://vnoi.info/wiki/translate/topcoder/dynamic-programming.md
> https://howkteam.vn/course/cau-truc-du-lieu-va-giai-thuat/quy-hoach-dong-4394

##### ***`Thuật toán, cấu trúc dữ liệu phức tạp: Cấu trúc dữ liệu`***

> **Segment Tree (Cây phân đoạn):**
> https://vnoi.info/wiki/algo/data-structures/segment-tree-basic.md
> https://vnoi.info/wiki/algo/data-structures/segment-tree-extend.md

> **Binary Indexed Tree (Cây chỉ số nhị phân):**
> https://vnoi.info/wiki/algo/data-structures/fenwick.md
> https://www.geeksforgeeks.org/binary-indexed-tree-or-fenwick-tree-2/

> **DSU (Disoint Set Union):**
> https://vnoi.info/wiki/algo/data-structures/disjoint-set-union.md
> https://howkteam.vn/course/cau-truc-du-lieu-va-giai-thuat/tong-quan-ve-disjoint-sets-union-va-cach-xay-dung-dsu-4385

> **Bài toán đồ thị:**
> https://vnoi.info/wiki/algo/graph-theory/everything.md
> https://v1study.com/c-plus-plus-reference-thuat-toan-do-thi-voi-c-plus-plus.html

***P/S: Tài liệu mang tính tham khảo, tốt nhất nên tìm hiểu thêm ở các nguồn khác.***