# EchoRead — Data Structure

## 1. User

```json
{
  "id": "uuid",
  "email": "user@example.com",
  "created_at": "2026-05-06T10:00:00Z"
}
```

## 2. Article

```json
{
  "id": "uuid",
  "user_id": "uuid",
  "title": "My Practice Article",
  "text": "The global healthcare industry...",
  "sentences": [
    "The global healthcare industry is entering a new era."
  ],
  "created_at": "2026-05-06T10:05:00Z"
}
```

## 3. Practice Session

```json
{
  "id": "uuid",
  "user_id": "uuid",
  "article_id": "uuid",
  "completed_sentences": 10,
  "highlight_words": ["era", "driven", "healthcare"],
  "created_at": "2026-05-06T10:20:00Z"
}
```

## 4. Sentence Practice

```json
{
  "id": "uuid",
  "session_id": "uuid",
  "sentence_index": 2,
  "original_sentence": "The global healthcare industry is entering a new era.",
  "recognized_text": "The global health care industry is entering a new area.",
  "feedback": {
    "encouragement": "这一句完成得很好。",
    "highlight": "整体节奏比较连贯。",
    "suggestion": "era 可以再轻一点，不要读成 area。"
  }
}
```

## 5. Review Word

```json
{
  "id": "uuid",
  "user_id": "uuid",
  "session_id": "uuid",
  "word": "era",
  "source_sentence": "The global healthcare industry is entering a new era.",
  "created_at": "2026-05-06T10:25:00Z"
}
```

## 6. MVP 暂不保存

- 录音文件
- 分数
- 排名
- 社交关系
- 长期学习画像
