# テーブル設計

## usersテーブル

| Column | Type   | Options      |
| name   | string | unique: true |

### Association

## roomsテーブル

| Column | Type   | Options |
| name   | string | ------- |

### Association

## messagesテーブル

| Column  | Type       | Options |
| content | text       | ------- |
| user    | references | null: false, foreign_tey: true |
| room    | references | null: false, foreign_tey: true |

### Association

belongs_to :user
belongs_to :room