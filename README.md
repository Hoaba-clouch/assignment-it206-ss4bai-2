# BÀI TẬP: Viết User Story, Acceptance Criteria và theo dõi trên Trello (ứng dụng đặt lịch khám RikkeiCare)

## Bước 1. Viết User Story cho R5

**Yêu cầu R5:** "Phòng khám muốn tự cập nhật giá các gói khám."

**User Story:** Là một **quản lý phòng khám**, tôi muốn **tự cập nhật giá các gói khám của mình**, để **đảm bảo thông tin giá luôn chính xác và linh hoạt theo thị trường**.

**Giải thích vai trò:** Tôi chọn vai trò "quản lý phòng khám" vì họ là người trực tiếp sử dụng tính năng này để điều chỉnh giá gói khám. "Admin RikkeiCare" chỉ là người đang thực hiện hộ, không phải là người sở hữu nhu cầu kinh doanh hay người hưởng lợi trực tiếp từ việc tự chủ động cập nhật giá. Việc trao quyền cho quản lý phòng khám tự cập nhật giá sẽ mang lại lợi ích trực tiếp cho phòng khám và giảm tải cho admin RikkeiCare.

## Bước 2. Viết phần Then cho 2 AC của R5

**AC 1 (thành công):** Given quản lý phòng khám đã đăng nhập, When nhập giá mới cho một gói khám rồi nhấn "Lưu", Then **hệ thống lưu thành công giá mới của gói khám và hiển thị giá mới đó trên trang quản lý gói khám của phòng khám.**

**AC 2 (thất bại):** Given quản lý để trống ô giá, When nhấn "Lưu", Then **hệ thống hiển thị thông báo lỗi "Giá không được để trống" và không lưu thay đổi.**

## Bước 3. Thẻ R5 đã sẵn sàng chưa?

Để đánh giá thẻ R5 đã sẵn sàng cho Sprint hay chưa, ta đối chiếu với Definition of Ready (DoR) của nhóm:

*   **Có User Story đủ 3 vế:** Có. User Story của R5 đã được viết đủ 3 vế (Là một <vai trò>, tôi muốn <nhu cầu>, để <lợi ích>).
*   **Có tiêu chí nghiệm thu:** Có. R5 đã có 2 Acceptance Criteria được viết theo mẫu Given – When – Then, bao gồm cả trường hợp thành công và thất bại.
*   **Đã được ước lượng:** Có. Theo dữ kiện ở Bước 5, thẻ R5 được ước lượng là 3 point.
*   **Đủ nhỏ để làm xong trong 1 Sprint:** Có. Với 3 point, R5 được coi là đủ nhỏ để hoàn thành trong một Sprint (Sprint dài 10 ngày với tổng cam kết 30 point).

**Kết luận:** Thẻ R5 **đã sẵn sàng** để được kéo sang cột "Ready for Sprint" vì nó đáp ứng đầy đủ cả 4 điều kiện trong Definition of Ready của nhóm.

## Bước 4. Hoàn thiện thẻ R5 trên Trello

*   **Nhãn:** Xanh dương (Feature) - Vì R5 là một tính năng mới cung cấp khả năng tự cập nhật giá cho quản lý phòng khám.
*   **Người phụ trách:** (Chưa được chỉ định cụ thể, giả định là một Developer) Ví dụ: Developer A
*   **Checklist (2–3 mục):**
    *   [ ] Thiết kế giao diện người dùng cho phần cập nhật giá gói khám
    *   [ ] Triển khai chức năng backend để lưu trữ và cập nhật giá gói khám
    *   [ ] Phát triển chức năng frontend để hiển thị và tương tác với việc cập nhật giá
    *   [ ] Viết kiểm thử tự động cho chức năng cập nhật giá
*   **Hạn hoàn thành:** (Ví dụ) Ngày thứ 7 của Sprint (nếu Sprint bắt đầu vào ngày 1, hạn là ngày 7).
*   **Vị trí trong cột:** Nếu R5 là việc ưu tiên cao nhất trong Sprint, thẻ sẽ được đặt ở **trên cùng** trong cột "Sprint Backlog".

## Bước 5. Đọc Burndown Chart

### a) Ngày 6 nhóm nhanh hay chậm so với đường lý tưởng, lệch bao nhiêu point?

*   **Tổng cam kết:** 30 point
*   **Số point giảm lý tưởng mỗi ngày:** 30 point / 10 ngày = 3 point/ngày.
*   **Số point lý tưởng còn lại vào Ngày 6:** 30 - (3 point/ngày * 6 ngày) = 30 - 18 = 12 point.
*   **Số point thực tế còn lại vào Ngày 6:** 20 point.

**So sánh:** Số point thực tế còn lại (20) lớn hơn số point lý tưởng còn lại (12). Do đó, nhóm đang **chậm** so với đường lý tưởng.

**Lệch:** 20 - 12 = **8 point**.

### b) Một bạn báo thẻ R5 "xong 80%" và muốn trừ luôn 3 point khỏi biểu đồ. Có nên không, vì sao?

**Không nên.**

**Giải thích:** Theo nguyên tắc Agile/Scrum và Definition of Done (DoD) của nhóm, điểm (point) chỉ được trừ khỏi Burndown Chart khi một hạng mục công việc (User Story hoặc Task) thực sự đã hoàn thành 100% và đáp ứng tất cả các tiêu chí "Done". Việc trừ điểm dựa trên phần trăm hoàn thành (ví dụ: 80%) là không phù hợp vì nó không phản ánh chính xác tiến độ hoàn thành giá trị có thể chuyển giao và có thể che giấu các rủi ro hoặc công việc còn lại. Chỉ khi thẻ R5 đáp ứng đầy đủ Acceptance Criteria và các điều kiện của Definition of Done, thì 3 point của nó mới được trừ khỏi biểu đồ Burndown.