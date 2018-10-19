![Demo Webdesign from this package](https://github.com/trantoan960/css-structure-rhp/blob/develop/build/images/bg.PNG)



# Front-End Architecture RHP Team 

<a href="https://github.com/trantoan960/css-structure-rhp"><img
  src="https://github.com/trantoan960/NguyenGiaWebsite.vn/blob/master/skyalbert.jpeg" alt="Normalize Logo"
  width="80" height="80" style="border-radius: 50%" align="right"></a>

> Một mini-project thuộc RHP Team. Bộ khung Front-End được nhóm thiết kế để người lập trình viên rút ngắn thời gian xây dựng trang web và giúp trang web có quy củ hơn. Sản phẩm cũng là món quà gửi tới các chị em thuộc nhóm RHP Team.



**Cài đặt**

```sh
Package này sẽ được update sớm lên npm để mọi người sử dụng dễ dàng hơn. Còn ở hiện tại, vui lòng clone để sử dụng.
```

**Ý tưởng**

See https://facebook.com/tran.toan.960

**Tải về**

See https://github.com/trantoan960/css-structure-rhp


## Bạn làm được gì từ package này.

* Code luôn và ngay mà không cần khởi tạo folder, file.
* Package hỗ trợ sẵn các cấu trúc folder, file giúp lập trình viên giảm ngắn thời gian code.
* Package hỗ trợ sẵn việc viết scss/sass. Việc của bạn là viết còn package sẽ gen code.
* Lựa chọn đầu ra đủ thứ bạn cần: .css, .min.css, .js, .min.js
* Trình duyệt tự động Reload khi bạn :D Ctrl + S
* Tích hợp sẵn gen ico tự động cho trang web.
* Khi viết CSS bạn không phải lo vì trình duyệt có tương thích không, package tích hợp sẵn prefix để tự động thêm tiền tó CSS thích hợp.
* Vân vân và mây mây...


## Trình duyệt hỗ trợ

* Chrome
* Edge
* Firefox ESR+
* Internet Explorer 10+
* Safari 8+
* Opera

## Editor khuyên dùng

* Visual Studio Code [Tải tại đây](https://code.visualstudio.com/)
* Atom (Package: Terminal) [Tải tại đây](https://atom.io/)

## Hướng dẫn sử dụng (Sass/Scss)

Package thực chất là kết hợp của nhiều package khác và config lại. Bạn phải có Nodejs trong máy tính. Nếu chưa có vui lòng tải [tại đây](https://nodejs.org/en/). Việc tải xuống và cài đặt với Node JS không có gì khó khăn cả. Cứ next, next nữa, next mãi thôi :))

> Chú ý: Bạn đã tải folder css structure về rồi nhé, clone, download tùy ý bạn.

**Bước 1**
```sh
npm install
```

Bước này để cài đặt các package cần thiết có trong package. Vui lòng không chỉnh sửa nội dung file package ở mục devDependiences. Bạn có thể thêm, xóa, còn sửa thì chỉ khi bạn đã hiểu bạn mới nên sửa đó là lời khuyên của mình.

**Bước 2**
```sh
gulp
```

Nếu là lần đầu bạn tải nodejs về, nó sẽ hỏi bạn cấp quyền bạn cho phép là được, từ lần sau cứ vậy là nó chạy trên trình duyệt. Công việc của bạn bây giờ là code thôi :)) Dễ dàng và easy.

## Hướng dẫn sử dụng (Code thuần)

Package này mình cũng đã tích hợp load trực tiếp như server vì thế, mọi ng vẫn thực hiện hai bước trên như bình thường. Khi code bạn code trực tiếp tại Folder build/.... 


## Cấu trúc folder

Folder ```build```:

* Scripts: Folder này chứa mã code JS mà bạn code, nên nhớ code ở folder này là tự gen bạn không phải làm gì.
* Styles: Folder này chứa mã code CSS mà bạn code, nên nhớ code ở folder này là tự gen bạn không phải làm gì.
* Videos, Images, Fonts,... còn lại: là source của bạn thôi, bạn thêm vào như bình thường :)) nếu trang web bạn cần.

Folder ```src```;

* Scripts: Trong folder này có một file tên là ```main.js``` bạn sẽ có JS ở đây. Trong folder còn thư mục vendors là thư mục để bạn đưa các thư viện bên ngoài vào liên quan tới JS. Chú ý nếu bạn dẫn link tới file main.min.js thì bạn không cần quan tâm tới việc thêm các đường dẫn file khác. package tự động gen thư viện trong foler vendors :D
* Styles: Trong folder này có file main.scss và 5 Folder đã được mình chia rất rõ ràng, nó là hợp lí cho cá nhân và một số thành viên đã sử dụng và cho kết quả lại cho hay. Bạn có thể tạo thêm file tùy ý bạn nhưng bạn nên theo quy tắc bên dưới sẽ dễ dàng hơn cho bạn.

**Quy tắc tạo file trong Styles**

* 0-plugins: là đoạn code css thư viện mà bạn add từ bên ngoài, cố gắng đặt tên theo ngữ nghĩa, mình đã đặt một số tên file trong đó, bạn có thể tham khảo.
* 1-helpers: là thư mục chứa viến, mixin, functions trong sass/scss, mình khuyến cáo nên giữ nguyên folder này như vậy là đầy đủ, không nên thêm file nào cả.
* 2-bases: là thư mục chứa các file về reset, global css, font chữ, kiểu chữ. Mình cũng đã tạo sẵn các file bạn có thể tham khảo.
* 3-layouts: là thư mục chứa code các phần của website ví dụ: header, fotter, main, nav,... Mình cũng đã tạo sẵn một số file.
* 4-modules: là thư mục chứa các code phần component như: button, card, box,.... Mình cũng đã tạo sẵn một số file.
* 5-tempaltes: là thư mục chứa các code của các trang ví dụ: home, contact, about, faq,... Mình cũng đã tạo một số file.


## Contributing

Please use code with free target, Source code take it with [Sky Albert](https://facebook.com/tran.toan.960) and RHP Team Members. You can join our team to talk something about code or anything else. [Please join, take it](https://discord.gg/UnZ4QTJ).

