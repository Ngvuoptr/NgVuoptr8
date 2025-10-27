---
name: Custom issue template
about: ".github/ISSUE_TEMPLATE/feature_request.md"
title: ''
labels: help wanted
assignees: Ngvuoptr

---

tên: Báo cáo lỗi
mô tả: Gửi báo cáo lỗi.
tiêu đề: "[Lỗi]: "
nhãn: ["lỗi", "phân loại"]
dự án: ["octo-org/1", "octo-org/44"]
người được giao nhiệm vụ:
  - mèo octocat
loại: lỗi
thân hình:
  - loại: markdown
    thuộc tính:
      giá trị: |
        Cảm ơn bạn đã dành thời gian điền vào báo cáo lỗi này!
  - loại: đầu vào
    id: liên hệ
    thuộc tính:
      nhãn: Chi tiết liên lạc
      Mô tả: Chúng tôi có thể liên lạc với bạn bằng cách nào nếu chúng tôi cần thêm thông tin?
      chỗ giữ chỗ: ví dụ: email@example.com
    xác thực:
      bắt buộc: sai
  - loại: vùng văn bản
    id: chuyện gì đã xảy ra
    thuộc tính:
      label: What happened?
      description: Also tell us, what did you expect to happen?
      placeholder: Tell us what you see!
      value: "A bug happened!"
    validations:
      required: true
  - type: dropdown
    id: version
    attributes:
      label: Version
      description: What version of our software are you running?
      options:
        - 1.0.2 (Default)
        - 1.0.3 (Edge)
      default: 0
    validations:
      required: true
  - type: dropdown
    id: browsers
    attributes:
      label: What browsers are you seeing the problem on?
      multiple: true
      options:
        - Firefox
        - Chrome
        - Safari
        - Microsoft Edge
  - type: textarea
    id: logs
    attributes:
      label: Relevant log output
      description: Please copy and paste any relevant log output. This will be automatically formatted into code, so no need for backticks.
      render: shell
  - type: checkboxes
    id: terms
    attributes:
      label: Code of Conduct
      description: By submitting this issue, you agree to follow our [Code of Conduct](https://example.com).
      options:
        - label: I agree to follow this project's Code of Conduct
          required: true
