# locale-vi-VI

Repo này chứa các tệp tiếng Việt cho các bản khảo sát State of JS/CSS/v.v. Bạn có thể xem danh sách [các ngôn ngữ tại đây](https://github.com/orgs/Devographics/repositories?q=locale&type=all&language=&sort=).

## Làm thế nào để giúp đỡ

#### 1. Trở thành dịch giả

Để bắt đầu giúp dịch khảo sát, bạn nên [tham gia Discord](https://discord.com/invite/zRDb35jfrt) và gửi tin nhắn trực tiếp cho tôi (`SachaG`) username GitHub của bạn, cùng với mã ngôn ngữ (`vi-VN`) mà bạn muốn trợ giúp.

Sau đó, tôi sẽ cấp cho bạn quyền bảo trì đối với repo này và từ giờ trở đi, bạn có thể tự mình quản lý nó cùng với các thành viên khác trong nhóm dịch.

Nếu bạn không tham gia nhóm Discord, bạn cũng có thể vào trang [issue](https://github.com/Devographics/locale-vi-VN/issues) để xem các file nào đang cần ưu tiên dịch, và có thể bắt đầu dịch. Với cách này, bạn sẽ cần yêu cầu 1 thành viên khác review và merge file dịch của bạn.

#### 2. Tìm những thứ cần dịch

Bạn có thể xem bên trang thực hiện khảo sát, hoặc trang web kết quả khảo sát, v.v. và tìm các câu chưa được dịch hoặc sử dụng API của chúng tôi để nhận thêm dữ liệu, chẳng hạn như tỷ lệ phần trăm hoàn thành cho một ngôn ngữ hoặc danh sách tất cả các chuỗi chưa được dịch:

- https://graphiql-internal.devographics.com/

Đây là một query mẫu:

```graphql
query GetLocaleData {
  locale(localeId: "ru-RU") {
    completion
    totalCount
    translatedCount
    translators
    untranslatedKeys
  }
}
```

#### 3. Nhận Credit

Mọi dịch giả sẽ được ghi tên trên bất kỳ trang web nào sử dụng bản dịch, trước tiên là với ứng dụng thực hiện khảo sát. Mặc dù điều này cuối cùng sẽ được tự động hóa thông qua API GitHub, nhưng hiện tại bạn có thể thêm tên của mình tại đây:

- https://github.com/devographics/monorepo/blob/main/api-internal/src/data/locales.yml

#### 4. Đưa bản dịch của bạn lên product

Hiện tại không có hook tự động để cập nhật lên product khi bản dịch được cập nhật. Vì vậy, cách tốt nhất hiện tại là gửi tin nhắn trực tiếp cho tôi trên Discord để cho tôi biết khi nào bạn hoàn tất.

## Các file cần dịch

#### Trang khảo sát

Các chuỗi này có liên quan đến trang mà bạn sử dụng để điền vào bản khảo sát thực tế.

- `surveys.yml`
- `accounts.yml`
- `state_of_js_2020_survey.yml`

#### Trang kết quả

Các chuỗi này chỉ xuất hiện trong trang hiển thị kết quả khảo sát và số liệu thống kê.

- `results.yml`
- `state_of_css_2020.yml`
- `state_of_js_2020.yml`

#### Cả hai

Những chuỗi này xuất hiện trong cả hai.

- `common.yml`
- `state_of_css.yml`
- `state_of_js.yml`

#### Khác

- `homepage.yml`

## Tham gia nhóm dịch thuật

Bạn nên tham gia [nhóm dịch thuật](https://github.com/orgs/StateOfJS/teams/translators/teams) cho ngôn ngữ bạn muốn dịch.

## Local Development

Hiện tại không có cách nào dễ dàng để xem kết quả dịch của bạn tại máy local. Chúng tôi đang cố gắng thực hiện nó.

## Tìm sự giúp đỡ

Tham gia [nhóm của chúng tôi trên Discord](https://discord.gg/zRDb35jfrt).
