- **BEWARE**: 
	- First thing should be done: mail all department to update statistics
- Note:
	- Packout: cutoff yesterday >< shipment: cutoff today.
	- Shipment: Can cut off yesterday in case of negative number.
a247: c to c. Hanking (hard cardboard)
B825: FATP
packout: cutoff yesterday vs shipment: can cutoff today. Because packout is based on report yesterday, but shipment have planned and can be sent today

PSD (mon[before 2pm] tue fri): cumulate B825 vs a247
	cumulative from beginning to end 
	packout (product and pack) input output, shipment (send number, including FD [forwarder] and DS [direct ship to retailer])
	-input (=packout, input must be equal to packout): find ke hoach sx (Thu: 29748). pp3 ramp plan & IOS 
	Shipment: ke hoach xuat hang (B825: Nguyet Anh - Alina; A247 Nga - Linzy)
	BOH: by on hand (in inventory)
		newest BOH: yesterday PK - today shipment
			Never a negative number (error)
	MP BOQ (multipack by on hand quarter)
			cut off each quarter (cut off CQ should be PK - shipment in that CQ)
	CW( current week)
	MP: multipack (x10/box)
	SP:singlepack (x1/box)
	gmail: alima, linzy, VN-PP3, PP2
		Cập nhật dữ liệu: packout, PO short,, PSD+, 
	PITS
		Nhớ Check đồng bộ (sum từng ngày và sum từ đầu đến ngày hiện tại, check với báo cáo gửi đến
	Sdm:supply demand management 
	In case input have trouble, send CTB report with capture SP will be supply plan
- Retrieving Data for writing reports
	- PSD+ PO shortage yyyymmdd
	- "Gửi mọi người, cập nhật dữ liệu Packout, PO shortage, PSD+, Shipment plan, shipment report gửi trước 10h
- PSD step-by-step:
1. Duplicate and put to new folder (For back-up, leave it at least for 2Q)
2. Take from PP2 (A247) (PSD+ PO shortage yyyymmddA-A247 PSD - PSD summary yyyymmdd.xlsx)
3. Take from PP3 (B815) (PSD+ PO shortage yyyymmddA-SHIP REPORT 825 - PSD summary yyyymmdd.xlsx) -> shipment data
4. Every Monday, Take PSD summary from mon-saturday. Then check sum and cum
5. Take Ramp plan pp2 and pp3 for Packout
	1. Go to PK ramp, 產出
6. Take ship report
	1. A247: Linzy (Nga)
	2. B825: Alina (Nguyệt Ánh là)
7. Take data from ship report
	1. Filter in heading rows
	2. Filtet MPN
	3. Filtet ship mode
	4. Filter ship type
	5. Calculate sum of Shipped Qty
	6. Check sum daily (ww summary), cum -> check sum every MPN
	7. Check day ship qty and cum ship all
8. Check #1 
	1. Ship report data compare (today's shipment and cum shipment) shipment data from [[Ramp plan]]
9. Check packout sum before closing
10. Check #2 
	1. Check number from Cum Output Actual (if PSD 19, IOS is 19-1=18) [[IOS]] [[PSD Summary]]
11. Update data B825 and A247 with each code
	1. Check sum data from PSD vs Ship report
	2. If product have same NP and shipment type, merge
12. Check BOH
	1. inventory = packout - shipment -> check gap -> take fill from B825+A247
	2. Copy today -1 to keep planning numbers, type today statistic manually
	3. Check inventory sum (**IMPORTANT**)
13. Open format of customer (B825+A247) (do not left blank in cells)
	1. Actual and Projection upload
		1. Change date CW ( from cw-1 to cw+4) for MP and SP. Cus in week, there might have changes
	2. Copy VALUE ONLY (CW and sum)
	3. Inventory Upload taken from BOH PSD internal
14. (If monday)
	1. packout plan based on Ramp plan (latest of both B825 and A247, even though none is sent today)
	2. Copy PK ramp zhanchu (line 3), copy EACH MPN individually (for B825 and A247). From Current date -> CW + 4
15. Upload
	1. delete history data
	2. partner.apple.com
	3. PSD plus -> FXVY - ACCY -> CW -1 to +4 -> PM -> view history and check status
	4. (If error) Restatement
