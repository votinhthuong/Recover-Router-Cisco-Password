*Các bước khôi phục mật khẩu cho router*

**Step 1: Tắt/mở router**

**Step 2: Nhấn Ctrl + Break để vào mode rommon**

**Step 3: Đổi giá trị thanh ghi cấu hình**
rommon 1 > confreg 0x2142

rommon 2 > reset

** Step 4: Sửa password**

Router# copy startup-config running-config

Router# conf t

Router(config)# enable password <mật_khẩu>

Router(config)# end

Router# wr

**Step 5: Đổi lại giá trị thanh ghi cấu hình**

Router(config)# config-register 0x2102

Router(config)# end

Router# end

Router# reload



