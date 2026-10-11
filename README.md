# Session 11 - Homework Ex2: Đóng gói JAR và lưu Artifacts

Kế thừa Ex1, bổ sung 2 bước vào Job `test` trong `.github/workflows/ci.yml:25`:

- `./gradlew bootJar` để đóng gói `build/libs/*.jar`
- `actions/upload-artifact@v4` với `name: app-jar`, `path: build/libs/*.jar`

## Kiểm tra
Push lên `main`, mở tab Actions → Summary, xác nhận có artifact `app-jar` tải về được.
