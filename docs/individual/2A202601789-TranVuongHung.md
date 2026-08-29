# Bài làm cá nhân — Trần Vương Hưng · `2A202601789`

**Nhóm JCungDuoc** · Dự án **MedTriage AI** · Day 27 · 29/08/2026
**Vai trò dự án:** AI / Platform Engineer — **chủ trì Phase 3 (AI Team Design), giữ nhịp Phase 5**

> File này chứa **phần tôi tự làm trước khi thảo luận** ở Phase 1.1, Phase 2.3 và Phase 4.1.

---

## Phase 1.1 — Stakeholder tôi tự liệt kê (5 phút, chưa thảo luận)

Tôi liệt kê được **7 stakeholder**. Góc nhìn của tôi nghiêng về **đường đi của dữ liệu và của hệ thống** —
đúng thói quen từ Day 22, khi tôi phải vẽ system boundary cho một hệ `semi-automated` có harm không đảo ngược được.

| # | Stakeholder tôi ghi | Influence | Interest | Stance tôi đoán | Vào bản đồ chung? |
|---|---|---|---|---|---|
| 1 | **Trưởng phòng CNTT / quản trị HIS bệnh viện A** — chủ HL7, chủ VPC, chủ dữ liệu | Cao | Thấp | **Chưa ủng hộ** | ✔ **S4** — *tôi là người duy nhất ghi ra* |
| 2 | **Nhà cung cấp HIS đương nhiệm của bệnh viện A** | Cao | Thấp | Trung lập | ✔ **S7** — *tôi là người duy nhất ghi ra* |
| 3 | Trưởng khoa Cấp cứu bệnh viện A | Cao | Cao | Trung lập | ✔ **S1** |
| 4 | Ban Giám đốc bệnh viện A | Cao | Thấp | Chưa ủng hộ | ✔ **S2** |
| 5 | Giảng viên / mentor Track 1 | Cao | Cao | Ủng hộ | ✔ **S5** |
| 6 | Nhà cung cấp mô hình / API LLM (đơn vị nhóm đang mua token) | Trung bình | Thấp | Trung lập | ✘ **loại** |
| 7 | Đơn vị hạ tầng đám mây | Thấp | Thấp | Trung lập | ✘ **loại** |

**Tôi tự loại #6 và #7** khi vào phần Team. Cả hai là **nhà cung cấp**, không phải stakeholder theo nghĩa của
Lab: họ không ảnh hưởng tới kết quả dự án và cũng không bị ảnh hưởng bởi nó — họ chỉ bán dịch vụ theo hợp đồng.
Giữ lại chỉ làm loãng bản đồ. (Rủi ro chi phí token thì đã có luật **R-05** ở dashboard Day 26 lo, không cần
một ô trên stakeholder map.)

### Điểm tôi đóng góp riêng và điểm tôi thiếu

**S7 — nhà cung cấp HIS đương nhiệm** là stakeholder mà cả Việt lẫn Linh đều không nghĩ tới, và nó **có hai mặt**:
vừa là cửa phải đi qua để tích hợp, vừa là **kênh phân phối của Plan B** mà chính nhóm đã viết trong kill criteria
ngày 26/11 ở Day 26 — *"chuyển bộ sinh SBAR + eval sang bán cho nhà cung cấp HIS dưới dạng module"*. Một stakeholder
nằm ở cả kịch bản thành công lẫn kịch bản thất bại thì không được để ngoài bản đồ.

**Thứ tôi thiếu:** danh sách của tôi **không có một người dùng cuối nào** — không có điều dưỡng, không có bệnh nhân.
Tôi liệt kê được đủ người giữ cửa hệ thống nhưng không có ai thực sự chạm vào sản phẩm. Đây là lỗ hổng cùng loại
với lỗ hổng của Việt, chỉ khác hướng.

---

## Phase 2.3 — Bản pitch tôi tự viết lại (5 phút)

> **Kết luận.** Đề nghị khoa cho MedTriage AI chạy **2 tuần ở chế độ chỉ ghi nhận**, đặt **một kiosk ở hàng chờ**,
> không kết nối vào bất kỳ hệ thống nào của bệnh viện, không xin tài khoản, không xin dữ liệu bệnh án.
>
> **Lý do.** (1) Vì không nối hệ thống nên khoa **không phải mở bất kỳ cửa nào** — không cần phòng CNTT, không cần
> phòng tài chính, không có thay đổi cấu hình nào để phải hoàn tác. (2) Dữ liệu được khử PII **trước khi rời VPC
> của bệnh viện**, và bệnh viện giữ quyền sở hữu toàn bộ phiếu SBAR sinh ra. (3) **Khoa giữ được kết quả kể cả khi
> khoa quyết định dừng** — nếu dừng giữa chừng, chúng tôi bàn giao toàn bộ ca đã gán nhãn và không giữ bản sao có PII.
>
> **Bằng chứng.** Chúng tôi đã đặt trước ngưỡng dừng cho cả chi phí lẫn an toàn, và có một cổng gác ngày 30 với
> tiêu chí viết sẵn. Chúng tôi **chưa có** số đo trên ca thật — đó chính là thứ 2 tuần này để lấy.
>
> **Small ask.** Cho chúng tôi đặt **một kiosk** ở hàng chờ trong 2 tuần, ca trực ngày. Chỉ cần một chỗ cắm điện
> và một chỗ đứng.

**Nhóm giữ lại từ bản của tôi:** câu **"khoa giữ được số đo kể cả khi khoa quyết định dừng"** — bản duy nhất
đưa ra thứ stakeholder được giữ trong **kịch bản xấu nhất**, và đó là thứ hạ rào cản đồng ý xuống thấp nhất.
Cùng với ý **"không phải mở bất kỳ cửa nào"**, đã thành phần *"không hợp đồng · không nối HIS · không ngân sách"*
trong bản cuối.
**Góp ý của tôi làm thay đổi bản của Việt:** bản gốc xin thêm *"quyền truy cập HIS ở chế độ chỉ đọc"*. Xin HIS là
kéo **S4** vào ngay từ tuần đầu — mà S4 là Blocker ảnh hưởng cao, quan tâm thấp, và không có động cơ nào để đồng ý
nhanh. Một small ask mà cần hai người gật đầu thì không còn là small ask. **Đã cắt.**

---

## Phase 3 — Phần tôi chủ trì: AI Team Design

Ba quyết định tôi đề xuất và bảo vệ trước nhóm:

1. **Chọn Embedded, không phải Hybrid.** Hybrid chỉ có nghĩa khi có năng lực **dùng lại được** giữa nhiều nơi.
   Nhóm có một sản phẩm và một khoa cấp cứu — mọi lớp trung gian đều làm chậm vòng học. Tôi ghi kèm **điều kiện
   chuyển sang Hybrid** (≥3 bệnh viện và ≥6 người) để đây là một quyết định có ngày hết hạn, không phải một cái nhãn.
2. **Gap G-2 (HL7/HIS) → Outsource theo gói, không Hire.** Đây là năng lực **dùng theo đợt**: nối xong một bệnh viện
   thì gần như không đụng tới cho tới bệnh viện sau. Tuyển full-time sẽ đẩy **chi phí triển khai ÷ ACV vượt trần
   24,4%** (phép tính MH-03 của Day 26) — đúng con số mà cổng ngày 60 đang gác. Tôi giữ điều kiện **nhóm sở hữu mã
   nguồn và tôi review**, để lần nối thứ hai rẻ hơn lần thứ nhất.
3. **Vai trò Domain Expert lâm sàng phải để trống và gọi đúng tên là gap.** Đề nghị ban đầu là chia đôi việc đó cho
   tôi và Linh. Tôi phản đối chính đề nghị có lợi cho mình: **không ai trong ba người là người hành nghề y**, và
   nhãn do người không hành nghề chốt thì bộ eval không có giá trị — cổng ngày 30 sẽ đo bằng thước do chính nhóm tự đúc.

---

## Phase 4.1 — Điểm Team Health tôi tự chấm (chưa nhìn điểm ai)

| Khía cạnh | Điểm tôi chấm | Tôi đang nhìn vào cái gì khi chấm |
|---|:---:|---|
| **Chất lượng AI** | **3** | Ở giữa Việt và Linh. Đường dữ liệu và kiến trúc thì đứng được, nhưng **chưa có gì chứng minh đầu ra đúng**. Chấm 3 vì phần tôi làm chạy được, phần chứng minh thì chưa. |
| **Tiến độ** | **3** | Bài nộp đúng hạn nhưng sản phẩm thì đứng yên — đó là hai loại tiến độ khác nhau. |
| **Tinh thần team** | **5** | Điểm cao nhất bảng, và tôi chấm có căn cứ: hôm nay tôi phản đối một đề nghị có lợi cho mình (nhận luôn vai Domain Expert) mà không ai coi đó là chuyện cá nhân. |
| **Tốc độ ra sản phẩm** | **3** | Tôi chấm cao hơn hai người kia 1 điểm vì tôi tính từ lúc có chữ ký: hạ tầng đã sẵn để dựng kiosk trong vài ngày. Nhưng sau khi nghe Linh, tôi công nhận **tốc độ phải đo tới người dùng thật**, mà tính như vậy thì hiện là vô hạn. |

### Sau khi so điểm

Tôi là người **chấm giữa** ở cả ba khía cạnh có chênh lệch — và điều đó không có nghĩa tôi đúng. Bài học của tôi
hôm nay: tôi đo tốc độ **từ chỗ tôi đứng** (hạ tầng sẵn sàng chưa) chứ không đo **tới nơi giá trị được nhận**
(người bệnh có được phân loại nhanh hơn không). Đo từ chỗ mình đứng luôn cho ra con số dễ chịu hơn thực tế.

---

## Phần tôi chịu trách nhiệm trong bài nộp

- **Trang 3 — AI Team Design:** toàn bộ — lựa chọn Embedded và điều kiện chuyển Hybrid, Core Roles, danh sách
  Extended cố ý chưa lập, và capability gap **G-2**.
- **Trang 1:** stakeholder **S4** và **S7** cùng lý do S7 nằm ở cả kịch bản thành công lẫn thất bại.
- **Trang 2:** đề xuất **tách R khỏi A** ở T3/T4/T5, và góp ý cắt phần "xin quyền truy cập HIS" khỏi small ask.
- **Chữ A trong RACI:** **T2** (dựng kiosk + pipeline khử PII trong VPC bệnh viện) và **T5** (vận hành shadow
  pilot 2 tuần tại khoa — uptime, thu ca, trực hỗ trợ tại chỗ).
- **Growth Plan:** owner của **G-3** — đặt nhịp **review 20 phút mỗi thứ Sáu 20h**, mỗi buổi có **đúng một người
  ngoài đội** dự (mentor tuần lẻ, cố vấn tài chính tuần chẵn), biên bản 5 dòng đẩy lên repo ngay sau buổi.
  Buổi đầu **05/09**, đủ 4 buổi trước **28/09/2026**. Tôi cũng là **người giữ nhịp cho điểm kiểm giữa kỳ ngày 14
  (12/09/2026)**.
- **Phase 5:** đọc checklist GATE 0 → GATE 5 cho cả nhóm tick từng ô (`docs/phase-gates.md`).
