---
name: Bug report
about: Create a report to help us improve
title: ''
labels: ''
assignees: ''

---

name: 🐛 Báo cáo lỗi (Bug Report)
description: Tạo báo cáo lỗi chi tiết giúp đội ngũ kỹ thuật xử lý nhanh hơn
title: "[Bug]: "
labels: ["bug", "triage"]
body:
  - type: markdown
    attributes:
      value: |
        Cảm ơn bạn đã báo cáo lỗi. Vui lòng cung cấp chi tiết theo mẫu bên dưới.

  - type: textarea
    id: description
    attributes:
      label: Mô tả lỗi
      description: Tóm tắt ngắn gọn lỗi đang xảy ra.
    validations:
      required: true

  - type: textarea
    id: steps
    attributes:
      label: Các bước tái hiện (Steps to Reproduce)
      description: Ghi rõ từng bước để tạo lại lỗi.
      placeholder: |
        1. Đi tới trang '...'
        2. Nhấn vào nút '....'
        3. Cuộn xuống màn hình '....'
    validations:
      required: true

  - type: textarea
    id: expected-actual
    attributes:
      label: Kết quả thực tế & Kết quả mong muốn
      placeholder: |
        - Mong muốn: ...
        - Thực tế xảy ra: ...
    validations:
      required: true

  - type: dropdown
    id: severity
    attributes:
      label: Mức độ nghiêm trọng
      options:
        - "Low (Lỗi giao diện nhỏ, không ảnh hưởng chức năng)"
        - "Medium (Tính năng hoạt động sai nhưng có cách khắc phục tạm thời)"
        - "High (Tính năng chính bị hỏng)"
        - "Critical / Blocker (Ứng dụng sập, mất dữ liệu, chặn toàn bộ flow)"
    validations:
      required: true

  - type: input
    id: environment
    attributes:
      label: Môi trường gặp lỗi
      placeholder: "Ví dụ: Chrome 124, Windows 11, App v1.3.0"
    validations:
      required: true

  - type: textarea
    id: logs-screenshots
    attributes:
      label: Ảnh chụp màn hình / Logs lỗi
      description: Kéo thả ảnh hoặc dán log console vào đây.
