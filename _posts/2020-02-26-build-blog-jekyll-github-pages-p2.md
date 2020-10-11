---
title: Hướng dẫn tạo blog miễn phí sử dụng Jekyll và Github Pages (P2)
date: 2020-02-26 20:55:00 +0700
categories: [Tutorial]
tags: [jekyll, tutorial, blog, web]
seo:
  date_modified: 2020-02-26 21:22:51 +0700
---

Xin chào các bạn, tiếp nối phần 1, chúng ta đã xây dựng được trang blog khá đẹp và chuyên nghiệp, ở phần 2 này mình sẽ hướng dẫn các bạn viết bài và publish lên blog, tối ưu tăng tốc độ load và setup một số công cụ theo dõi trang web.  

## Tạo bài mới
Để tạo được bài viết mới, bạn cần clone project về máy, sau đó mở bằng IDE bất kì, ở đây mình chọn VS Code.  
Bạn sẽ thấy có rất nhiều thư mục, trước hết bạn chỉ cần lưu ý thư mục **_post**, đây sẽ là nơi lưu giữ các bài post của bạn.  
Hãy tạo một file mới có tên như sau:  
*2020-02-26-build-blog-jekyll-github-pages-p2.md*
Mặc định các post sẽ xử lý các bài post dựa trên định dạng markdown, tên file bao gồm ngày tháng tạo, một slug mô tả ngắn về nội dung sẽ trình bày và phần đuôi .md (markdown).  
Mở đầu mỗi bài post bạn nên define các thành phần sau:  
- title: Tiêu đề bài viết
- date: Ngày viết bài
- categories: Các danh mục mà bài viết sẽ thuộc về
- tags: Gắn tags cho bài viết này
Việc define các thành phần trên rất quan trọng, giúp trang web của bạn SEO dễ dàng hơn, tạm thời bạn cứ đặt theo ý thích, việc đặt đúng chuẩn SEO có lẽ mình sẽ chia sẻ trong bài viết khác.  
Sau phần này sẽ là phần nội dung bài viết, đừng viết quá ngắn hoặc quá dài, viết vừa đủ để người đọc ko cảm thấy quá tải cũng như cảm thấy bài viết kém chất lượng.  
Để sử dụng ảnh trong bài viết thì bạn sẽ để ảnh vào thư mục **assets/img** và load vào trang là được, ví dụ như: 
*![domains-google]({{ "/assets/img/jekyll/domain.PNG" | relative_url }})*
Sau khi đã xong thì bạn publish lên github và reload lại blog là xong ! :D

## Tối ưu tốc độ load trang

Trong bài viết bạn sẽ sử dụng rất nhiều hình ảnh minh họa, nếu ảnh này ko được optimize dẫn tới kích thước ảnh lớn, load sẽ rất chậm.  
Rất may là có 1 công cụ rất hay và miễn phí đó là tinypng, bạn làm theo các bước sau để giảm kích thước ảnh nhé:  
- Truy cập https://tinypng.com/
- Upload ảnh cần optimize
- Chờ tinypng xử lý và tải về
Như vậy là bạn đã có những bức ảnh kích thước nhỏ gọn mà chất lượng ko tồi dành cho bài viết của mình. :D  

## Setup tool theo dõi blog

Có rất nhiều tool giúp việc monitor blog của bạn dễ dàng, nhưng mình khuyến khích bạn dùng google analytics, đây là một công cụ tuyệt vời và mạnh mẽ, hơn nữa lại hoàn toàn miễn phí.  
Bạn cần lập 1 tài khoản gmail và đăng nhập vào ứng dụng google analytic. Add tên miền trang blog

Sau đó bạn chỉ cần tải ứng dụng GG Analytics từ app store là có thể theo dõi lượng người truy cập trang blog của mình từ bất cứ đâu.  

Vậy là xong 2 bài chia sẻ của mình về quá trình mình tạo trang blog này, nếu có vướng mắc gì cứ comment mình sẽ giải đáp.  