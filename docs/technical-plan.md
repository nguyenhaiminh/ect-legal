# ECT Legal — Kế hoạch kỹ thuật

## Kiến trúc MVP

```text
Static UI (HTML/CSS/JS)
  ├─ question catalog (curated prompts)
  ├─ answer cards (curated, cited)
  ├─ legal source registry (version/effective state)
  └─ checklist (localStorage only)
```

## Kiến trúc giai đoạn 2

```text
Source connectors → raw documents → normalized legal registry → search index
                                      ↓
                               citation-aware RAG API
                                      ↓
                           UI + audit/version dashboard
```

## Data model tối thiểu

```json
{
  "id": "nd-23-2025",
  "title": "Nghị định 23/2025/NĐ-CP",
  "type": "nghi_dinh",
  "issued_at": "2025-02-21",
  "effective_at": "2025-04-10",
  "status": "in_force",
  "topics": ["electronic_signature", "trust_services"],
  "source_url": "https://vanban.chinhphu.vn/?docid=212829&pageid=27160",
  "last_verified_at": "2026-10-15"
}
```

## Quality gates

- Chặn deploy nếu nguồn không có URL chính thức hoặc thiếu ngày hiệu lực.
- Hiển thị cảnh báo khi `effective_at` ở tương lai.
- Citation bắt buộc trên mọi answer card.
- Tách dữ liệu nguồn khỏi nội dung trình bày để thay đổi UI không làm sai tri thức.
- Log phiên bản bộ luật, prompt và answer để tái hiện kết quả.
