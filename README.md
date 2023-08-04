FCA BY CANDY-DARKSTER 

## Important !

This package require NodeJS 14.17.0 to work properly.

## Notification !

+ We will have Example Video on Channel "Nguyễn Thái Hảo Official"

Original Project(Deprecated):

Chúc các bạn một ngày tốt lành!, cảm ơn vì đã sài Sản phẩm Candy, thân ái

KANZUWAKAZAKI(15/04/2023)

## Support For : 

+ Support English, VietNamese !,
+ All bot if using listenMqtt first.

# Api Cho ChatBot Messenger

Facebook Đã Có Và Cho Người Dùng Tạo Api Cho Chatbots 😪 Tại Đey => [Đây Nè](https://developers.facebook.com/docs/messenger-platform).

### Api Này Có Thể Khiến Cho Bạn Payy Acc Như Cách Acc Bạn Chưa Từng Có, Hãy Chú Ý Nhé =)

## Tải Về 

Nếu Bạn Muốn Sử Dụng, Hãy Tải Nó Bằng Cách:
```bash
npm i fca-candy-darkster
```
or
```bash
npm install fca-candy-darkster
```

Nó Sẽ Tải Vô node_modules (Lib Của Bạn) - Lưu Ý Replit Sẽ Không Hiện Đâu Mà Tìm 😪

### Tải Bản Mới Nhất Hoặc Update

Nếu Bạn Muốn Sử Dụng Phiên Bản Mới Nhất Hay Cập Nhật Thì Hãy Vô Terminal Hoặc Command Promt Nhập :
```bash
npm install fca-candy-darkster@latest
```
Hoặc
```bash
npm i fca-candy-darkster@latest
```

## Nếu Bạn Muốn Test Api 

Lợi Ích Cho Việc Này Thì Bạn Sẽ Không Tốn Thời Gian Pay Acc Và Có Acc 😪
Hãy Sử Dụng Với Tài Khoản Thử Nghiệm => [Facebook Whitehat Accounts](https://www.facebook.com/whitehat/accounts/).

## Cách Sử Dụng

```javascript
const login = require("fca-candy-darkster"); // lấy từ lib ra 

// đăng nhập
login({email: "Gmail Account", password: "Mật Khẩu Facebook Của Bạn"}, (err, api

    if(err) return console.error(err); // trường hợp lỗi

    // tạo bot tự động nhái theo bạn:
    api.listenMqtt((err, message) => {
        api.sendMessage(message.body, message.threadID);
    });

});
```

Kết Quả Là Nó Sẽ Nhái Bạn Như Hình Dưới:
<img width="517" alt="screen shot 2016-11-04 at 14 36 00" 

Nếu Bạn Muốn Sử Dụng Nâng Cao Thì Hãy Sử Dụng Các Loại Bot Được Liệt Kê Ở Trên !

## Danh Sách

Bạn Có Thể Đọc Full Api Tại => [here](DOCS.md).

## Cài Đặt Cho Mirai: 

Bạn Cần Vô File Mirai.js,Sau Đó Tìm Đến Dòng
```js
    var login = require('tùy bot'); 
    /* Có thể là :
        var login = require('@maihuybao/fca-Unofficial');
        var login = require('fca-xuyen-get');
        var login = require('fca-unofficial-force');
    ...   
    */
```

Và Thay Nó Bằng:

```js
    var login = require('fca-candy-darkster')
```

Sau Đó Thì Chạy Bình Thường Thôi  !

## Tự Nghiên Cứu

Nếu Bạn Muốn Tự Nghiên Cứu Hoặc Tạo Bot Cho Riêng Bạn Thì Bạn Hãy Vô Cái Này Đọc Chức Năng Của Nó Và Cách Sử Dụng

------------------------------------

### Lưu Lại Thông Tin Đăng Nhập.

Để Lưu Lại Thì Bạn Cần 1 Apstate Kiểu (Cookie, etc,..) Để Lưu Lại Hoặc Là Sử Dụng Mã Login Như Trên Để Đăng Nhập !

Và Chế Độ Này Đã Có Sẵn Trong 1 Số Bot Việt Nam Nên Bạn Cứ Yên Tâm Nhé !

__Hướng Dẫn Với Appstate__

```js
const fs = require("fs");
const login = require("fca-candy-darkster");

var credentials = {email: "FB_EMAIL", password: "FB_PASSWORD"}; // thông tin tk

login(credentials, (err, api) => {
    if(err) return console.error(err);
    // đăng nhập
    fs.writeFileSync('appstate.json', JSON.stringify(api.getAppState(), null,'\t')); //tạo appstate
});
```

Hoặc Dễ Dàng Hơn ( Chuyên Nghiệp ) Bạn Có Thể Dùng => [c3c-fbstate](https://github.com/c3cbot/c3c-fbstate) Để Lấy Fbstate And Rename Lại Thành Apstate Cũng Được ! (appstate.json)

------------------------------------

#
