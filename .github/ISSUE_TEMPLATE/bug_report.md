name: Hata Bildirimi
description: Oyun sırasında karşılaştığınız bir hatayı bildirin.
title: "[HATA] Kısa açıklama"
labels: [oyuncu-hatasi]
body:
  - type: markdown
    attributes:
      value: |
        ## 🔧 Hata Bildirim Formu

        Karşılaştığınız hatayı aşağıdaki alanları doldurarak bize bildirin. Teşekkür ederiz!

  - type: textarea
    id: what-happened
    attributes:
      label: Ne Oldu?
      description: Hatayı anlatın. Ne yaptığınızda ortaya çıktı?
      placeholder: Örneğin: "Evimin kapısından çıkarken oyun dondu."
    validations:
      required: true

  - type: input
    id: when
    attributes:
      label: Ne Zaman Oldu?
      placeholder: Örnek: 18 Mayıs 2025, saat 15:30 civarı
    validations:
      required: false

  - type: textarea
    id: how-to-reproduce
    attributes:
      label: Tekrar Ediyor mu?
      description: Aynı şeyi tekrar yapınca yine oluyor mu?
      placeholder: "Evet, her zaman oluyor / Hayır, bir kez oldu"
    validations:
      required: false

  - type: input
    id: player-name
    attributes:
      label: Oyuncu Adınız
      placeholder: Oyundaki karakter isminiz
    validations:
      required: false
