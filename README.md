# Website Trường TH, THCS và THPT Thực hành Sư phạm - Đại học Hạ Long

Website trường học hoàn chỉnh với hệ thống đăng ký tuyển sinh trực tuyến.

## 🆕 **Cập nhật mới nhất - Tháng 4/2026**

### ✅ **Đã thêm 3 trang đăng ký tuyển sinh:**

#### 📝 **1. Đăng ký vào lớp 1** - `dang-ky-lop-1.html`
- **Đối tượng**: Trẻ em đủ 6 tuổi vào lớp 1
- **Form đăng ký**: 
  - Thông tin cá nhân học sinh (họ tên, giới tính, ngày sinh, địa chỉ...)
  - Thông tin gia đình (cha mẹ, nghề nghiệp, liên hệ...)
  - Cam kết của phụ huynh
- **Tính năng**: 
  - Validation tự động (kiểm tra tuổi, số điện thoại...)
  - Tự động chuyển tên thành chữ HOA
  - Responsive design
- **Màu chủ đạo**: Xanh lục tươi (#22c55e)

#### 📚 **2. Đăng ký vào lớp 6** - `dang-ky-lop-6.html`
- **Đối tượng**: Học sinh hoàn thành chương trình tiểu học
- **Form đăng ký**:
  - Thông tin cá nhân học sinh
  - Thông tin học tập tiểu học (trường cũ, điểm TB, hạnh kiểm...)
  - Thành tích, giải thưởng (nếu có)
  - Thông tin gia đình
- **Yêu cầu**: 
  - Điểm TB lớp 5: từ 6.5 trở lên
  - Hạnh kiểm: Khá trở lên
- **Validation**: Kiểm tra điểm số, cảnh báo nếu dưới yêu cầu

#### 🎓 **3. Đăng ký vào lớp 10** - `dang-ky-lop-10.html`
- **Đối tượng**: Học sinh hoàn thành chương trình THCS
- **Form đăng ký phức tạp**:
  - Thông tin cá nhân (bao gồm số CCCD bắt buộc)
  - Kết quả học tập THCS (lớp 7, 8, 9)
  - Điểm chi tiết các môn Toán, Văn
  - Thành tích HSG các cấp
  - Thông tin gia đình
- **Yêu cầu cao**:
  - Điểm TB cả năm lớp 9: từ 6.5 trở lên  
  - Hạnh kiểm: Khá trở lên
  - Ưu tiên HSG và học lực Giỏi
- **Validation đầy đủ**: Kiểm tra tất cả yêu cầu tuyển sinh

### 🗂️ **Cấu trúc files mới:**

```
📁 Website Trường
├── 📄 index.html              # Trang chủ (đã cập nhật menu)
├── 📄 dang-ky-lop-1.html     # Form đăng ký lớp 1  
├── 📄 dang-ky-lop-6.html     # Form đăng ký lớp 6
├── 📄 dang-ky-lop-10.html    # Form đăng ký lớp 10
├── 🎨 style.css               # CSS (đã thêm dropdown)
├── ⚙️ script.js               # JavaScript cơ bản
└── 📖 README.md              # Hướng dẫn này
```

### 🎨 **Cập nhật giao diện:**

#### **Menu navigation mới:**
- **Dropdown "TUYỂN SINH"** với 3 mục con:
  - 👶 Đăng ký vào lớp 1
  - 🎒 Đăng ký vào lớp 6  
  - 🎓 Đăng ký vào lớp 10
- **Hiệu ứng hover**: Dropdown xuất hiện mượt mà
- **Icon**: Font Awesome icons cho từng cấp học

#### **Quick Links cập nhật:**
- Thay "Tuyển sinh 2025" → "Đăng ký lớp 1/6/10"
- **Clickable**: Mở trang đăng ký trong tab mới
- Giữ nguyên màu vàng cam (#f59e0b)

#### **Sidebar mới:**
- **Section "🎓 TUYỂN SINH NĂM HỌC 2025-2026"**
- **3 nút CTA nổi bật**:
  - 👶 Lớp 1 (xanh lục)
  - 🎒 Lớp 6 (xanh dương) 
  - 🎓 Lớp 10 (vàng cam)
- **Thông tin liên hệ**: Hotline và hạn nộp hồ sơ

#### **Tin tức cập nhật:**
- **Tin tuyển sinh** có link trực tiếp đến form đăng ký
- **Thông tin nổi bật**: Hotline, thời gian nộp hồ sơ
- **Style mới**: Box màu xanh nhạt với border trái

### 🛠️ **Tính năng kỹ thuật:**

#### **Responsive Design:**
- Tất cả 3 trang đăng ký responsive hoàn toàn
- Mobile-friendly từ 320px trở lên
- Flexbox layout tự động điều chỉnh

#### **Form Validation:**
```javascript
// Kiểm tra tuổi cho lớp 1
age >= 6 years

// Kiểm tra điểm số (0-10)
GPA validation với cảnh báo

// Kiểm tra số điện thoại (10-11 chữ số)
Phone regex: /^[0-9]{10,11}$/

// Kiểm tra CCCD (12 chữ số cho lớp 10)
Citizen ID: /^[0-9]{12}$/

// Consistency check
Thành tích <-> Giải thưởng phải tương ứng
```

#### **User Experience:**
- **Auto uppercase**: Tên học sinh tự động HOA
- **Smart placeholders**: Gợi ý thông minh
- **Error highlighting**: Border đỏ khi lỗi
- **Confirm dialog**: Xác nhận trước khi gửi
- **Reset function**: Xóa toàn bộ và reset style

### 📋 **Quy trình đăng ký:**

#### **Bước 1**: Chọn cấp học
- Từ menu dropdown "TUYỂN SINH"
- Hoặc click Quick Links  
- Hoặc từ sidebar CTA buttons

#### **Bước 2**: Điền form
- **Lớp 1**: Thông tin cơ bản + gia đình
- **Lớp 6**: + Kết quả tiểu học + thành tích
- **Lớp 10**: + Kết quả THCS 3 năm + HSG

#### **Bước 3**: Validation tự động
- Kiểm tra độ tuổi/học lực
- Validate format dữ liệu
- Cảnh báo nếu không đạt yêu cầu

#### **Bước 4**: Xác nhận gửi
- Dialog xác nhận cuối cùng
- Cam kết về tính chính xác thông tin

### 💡 **Điểm nổi bật:**

#### **✨ Design hiện đại:**
- Màu sắc tươi sáng, không gradient
- Card design với bo góc và đổ bóng
- Typography rõ ràng, dễ đọc
- Icon phù hợp từng cấp học

#### **⚡ Performance:**
- Pure HTML/CSS/JS, không framework
- Tải nhanh, runtime mượt
- Mobile optimization tốt
- Cross-browser compatible

#### **🎯 UX thông minh:**
- Progressive disclosure (ít → nhiều thông tin)
- Contextual help và gợi ý
- Error prevention tốt
- Clear call-to-actions

#### **📱 Accessibility:**
- Semantic HTML structure
- Keyboard navigation support  
- Screen reader friendly
- High contrast colors

### 🚀 **Cách sử dụng:**

#### **Cho phụ huynh:**
1. Truy cập website trường
2. Click menu "TUYỂN SINH" 
3. Chọn cấp học phù hợp
4. Điền đầy đủ thông tin
5. Kiểm tra và gửi đăng ký

#### **Cho nhà trường:**
1. **Nhận đăng ký**: Form data từ website
2. **Xử lý hồ sơ**: Kiểm tra thông tin
3. **Liên hệ xác nhận**: Qua hotline
4. **Thông báo kết quả**: Email/SMS

### 📞 **Thông tin liên hệ & Hỗ trợ:**

- **📍 Địa chỉ**: 258 Lê Thánh Tông, Phường Hồng Gai, TP. Hạ Long, Quảng Ninh
- **☎️ Hotline tuyển sinh**: 0203.3841.166  
- **✉️ Email**: thuchanh@uhl.edu.vn
- **🌐 Facebook**: /Truongthuchanhsupham

### 🔄 **Cập nhật tiếp theo:**

#### **Phase 2 có thể thêm:**
- [ ] Admin dashboard quản lý đăng ký
- [ ] Email confirmation tự động  
- [ ] Payment gateway học phí
- [ ] Parent portal theo dõi
- [ ] Calendar events tuyển sinh
- [ ] Multi-language support
- [ ] Advanced analytics
- [ ] Document upload feature

---

**🎉 Website đã sẵn sàng cho mùa tuyển sinh 2025-2026!**

*Phiên bản*: 3.0 - Full Admission System  
*Cập nhật*: April 2026  
*Tương thích*: All modern browsers, Fully responsive*# truongthuchanh
