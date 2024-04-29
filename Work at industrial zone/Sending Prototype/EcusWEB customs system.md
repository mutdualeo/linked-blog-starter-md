### Purpose: Control, record ALL in/out factory of materials/products 
DRI: Delivery control centre (Planning dept), Custom Dept, Logistic Dept, Material control, Purchasing dept...or any dept involving in material, product in/out access.
### EcusWEB Custom application
- http://ecusweb.efoxconn.com/vn/Login.aspx
	- Access in Factory
	- Access outside Factory
		- With customs declared (use PM acc to apply)
		- Without customs declared (Custom dept apply)
	- PM Ecus Web account:
		- ACC: V0236134
		- Password: Foxconn00* (change every 1 month)
	- 
- Hỗ trợ quản lý
	- **Product out of Factory**: "Cho phép xuất xưởng"
	- **Product into Factory**: "Cho phép vào xưởng"
-[ Xuất hàng ra ngoài xưởng - Không báo quan] (No Custom decleration)
	 - Thông tin chung: `Hàng xuất xưởng (không báo quan)`. If <10pcs, price is insignificant (~$10)
	 - Mã nhà xưởng: N
	 - Chủ quản duyệt: F0832374 (climber PM)
	 - Chủ quản cấp cao duyệt: F0519414 (Lu Zhong Fang)
	 - Người làm đơn chú thích: ID, name 
	 -  Phương thức vận chuyển: choose Nhân công -> don't need info related to car
	 - Loại hình xuất xưởng: Choose `085- hàng tạm xuất`
	 - Khu đóng hàng: where products is packed - 03 Bac Giang-Van Trung/北江－云中
	 - trọng lượng tịnh: not included packaging weight
	- loại hàng hóa: 2-Chưa khai báo
	- Phương thức đóng gói: BX-BOX (đóng gói ngoài cùng của hàng gửi)
	- địa chỉ dỡ hàng: giống địa chỉ người nhận
	- Mã liệu: FPN
	- Ghi chú: ID, Name, others request
	- Số đơn nguồn: Copy số đơn nguồn
	- Check info -> S.Lưu -> Xin xác nhận
	- If success -> 2. Đang ký duyệt ->3. Ký duyệt hoàn thành-> write `số đơn hàng` for guards to check (2 of 'em: in factory and A3) ->Y: gửi đi OR Z: Xin trả về + reason -> continue modify information (if any, cus after goards sign we cannot make further change)
	- For tracking: type `số đơn hàng/số đơn nguồn` -> `tất cả trạng thái` -> `tra cứu`
- Xuất hàng ra ngoài xưởng - Có báo quan
	- Số đơn nguồn: số tờ khai hải quan của đơn hàng xuất
	- loại hình xuất xưởng: 0002 -XK YP/ 国外出口成品
	- loại hàng hoá: 1- Có khai báo
	- Ngày rời xưởng dự kiến: must type even not exporting
	- Nơi giao hàng: Vân Trung
	- Loại hình vào xưởng: 004-Hàng tạm nhập (1)暂时进厂货物
	- Loại hàng khoá: `2_Chưa khai báo`
	- Use Custom Dep's acc or Plan Dep's to check, change, create requessts. PM acc can only do it in [Xuất hàng ra ngoài xưởng - Không báo quan]
	- Xin xác nhận (no need for confirmation)