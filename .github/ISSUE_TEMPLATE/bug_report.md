name: 不具合報告
description: 不具合報告フォーム
title: "[不具合]: "
labels: ["bug"]
assignees:
  - dninomiya
body:
  - type: markdown
    attributes:
      value: |
        不具合報告にご協力いただきありがとうございます
  - type: input
    id: contact
    attributes:
      label: Contact Details
      description: How can we get in touch with you if we need more info?
      placeholder: ex. email@example.com
    validations:
      required: false
  - type: textarea
    id: what-happened
    attributes:
      label: 不具合の詳細
      description: できるだけ具体的に記載をお願いします。できればスクリーンショットを添えてください。
      placeholder: __画面で__すると__が発生した
      value: ""
    validations:
      required: true
  - type: dropdown
    id: browsers
    attributes:
      label: どのブラウザをお使いですか？
      multiple: true
      options:
        - Chrome
        - Chrome(Android)
        - Safari
        - Safari(iOS)
        - Microsoft Edge
        - Firefox
