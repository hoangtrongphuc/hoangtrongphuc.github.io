---
title: Hướng dẫn tạo blog miễn phí sử dụng Jekyll và Github Pages (P1)
date: 2020-02-04 20:55:00 +0700
categories: [Tutorial]
tags: [jekyll, tutorial, blog, web]
seo:
  date_modified: 2020-02-04 16:43:05 +0700
---

Xin chào các bạn, hôm nay mình sẽ hướng dẫn các bạn cách tạo 1 trang blog cá nhân, từ A-Z với chi phí rẻ nhất và chất lượng khá ok :).
Mình sẽ hướng dẫn step-by-step, sau khi hoàn thành các bạn sẽ có 1 trang blog bao đẹp, bao an toàn (SSL), chỉ tốn khoản
phí để gia hạn tên miền (đắt hay rẻ tùy thuộc tên miền bạn chọn nha :v).

## Đăng kí tên miền

Đây là bước đầu tiên, chọn một tên miền cho blog. Bạn đừng nên đặt bừa một tên miền hoặc chọn tên miền quá hot vì chi phí sẽ rất cao (có tên miền cả chục ngàn đô cho 1 năm gia hạn) và ko tốt cho việc SEO và chạy quảng cáo sau này, nói ra thì dài dòng nhưng nếu là blog cá nhân thì nên chọn theo các tiêu chí: 
- Đuôi đẹp nhất là .com, nếu hết thì chọn .net hoặc .dev, .vn cũng ok.
- Tên miền ngắn gọn, súc tích, sử dụng chính tên của bạn như 1 số blogger nổi tiếng (thachpham.com, thekhuong.com), hoặc tìm một tên miền bắt tai (toidicodedao.com, codetips.vn).
- Nên chọn tên miền giá hạt rẻ, mới đầu thì tầm 500k/năm đổ lại là được, đừng cố quá mua những domain đẹp vì thực sự chất lượng bài viết của blog được đánh giá cao hơn là cái domain đẹp.

Để đăng kí tên miền thì có nhiều nhà cung cấp như goddady, namecheap... nhưng mình đang sử dụng và thấy hài lòng nhất là Google Domains, 1 dịch vụ do gg cung cấp, giao diện gọn gàng dễ sử dụng.

Bạn chỉ cần truy cập trang: **domains.google.com**, đăng nhập tài khoản gmail của bạn và tìm 1 tên miền mà bạn thích như hình dưới:
![domains-google]({{ "/assets/img/jekyll/domain.PNG" | relative_url }})
Đoạn này chỉ cần thêm vào giỏ hàng rồi mua là xong.

Tiếp theo là đến bước trỏ tên miền về dải IP của Github Pages.
Bên thanh menu trái, bạn chọn mục *DNS*, kéo xuống phần *Bản ghi tài nguyên tùy chỉnh*, bạn cấu hình một *A* record trỏ đến 4 địa chỉ IPv4 của Github Pages như hình dưới:
![a-record]({{ "/assets/img/jekyll/arecord.PNG" | relative_url }})
Vậy là xong bước 1, bạn đã có tên miền và trỏ tên miền này về dải IP của Github Pages, tiếp theo chúng ta sẽ tạo 1 trang Github Pages

## Tạo trang github pages

Bước này để tạo 1 trang github page bạn nên tìm 1 theme sẵn có, hoặc rảnh thì có thể tự tạo riêng một trang như trên trang [**jekyll.com**](https://jekyllrb.com/) có hướng dẫn.

Có nhiều trang web cung cấp các jekyll themes miễn phí, và ở đây mình chọn 1 theme trên [**https://jamstackthemes.dev/**](https://jamstackthemes.dev/). 

Khi chọn được theme yêu thích thì bạn truy cập trang github của theme này và fork về, phần này bạn nhớ đặt tên project có dạng *{username}.github.io* (username là tên github của bạn) vì đây là tên mà Github Pages sử dụng để deploy và tạo 1 domain tạm thời để bạn truy cập blog.

Sau khi hoàn tất bạn sẽ có 1 project như hình dưới: 
![fork]({{ "/assets/img/jekyll/fork.PNG" | relative_url }})

Tiếp theo bạn vào mục *Settings* của project và setup các thành phần sau:
- Tìm mục *Github Pages*, trong dropbox *Source* thì chọn master, đây là nhánh mà Github Pages sử dụng để deploy blog của bạn.
- Lúc này có hiện ra mục *Custom domain*, bạn nhập domain mà bạn vừa mua vào đó, Github Pages sẽ tự tạo 1 file CNAME để tạo custom domain cho bạn, nhớ đánh dấu cả vào *Enforce HTTPS*.

Sau khi hoàn tất bạn sẽ nhìn thấy thông báo như sau:
![pages]({{ "/assets/img/jekyll/pages.PNG" | relative_url }})

Tuyệt vời, vậy là bạn có thể truy cập domain bạn đã mua để hưởng thụ thành quả. 

1 trang blog khá ổn, có HTTPS và ko mất chi phí cho việc hosting :)

Phần 1 đến đây thôi, phần 2 mình sẽ hướng dẫn các bạn cấu hình Google Analytics và cách thêm bài viết mới sử dụng Jekyll.
