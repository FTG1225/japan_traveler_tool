# テーブル設計

## USERS テーブル
| column     | type    | options     |
| ---------- | ------- | ----------- |
| Nickname   | string  | null: false |
| Email      | string  | null: false |
| Password   | string  | null: false |
| Prefecture | integer | null: false |

### Association
- belongs_to_active_hash :prefecture

## WANT TO GO テーブル
| column      | type    | options     |
| ----------- | ------- | ----------- |
| Prefecture  | integer | null: false |
| Place       | string  | null: false |
| Date        | integer | null: false |
| Travel Time | integer | null: false |
| Destination | string  | null: false |
| Food        | string  |             |
| Hotel       | string  |             |
| Price       | string  |             |

### Association
- belongs_to_active_hash :prefecture

## REVIEW テーブル
| column      | type    | options     |
| ----------- | ------- | ----------- |
| Prefecture  | integer | null: false |
| Place       | integer | null:false  |
| Review      | integer | null:false  |

### Association
- belongs_to_active_hash :prefecture

## TRANSFER テーブル
| column     | type    | options     |
| ---------- | ------- | ----------- |
| Prefecture | string  | null: false |
| Transfer   | string  | null: false |
| Time       | integer | null: false |
| Price      | string  | null: false |

### Association
- belongs_to_active_hash :prefecture

## CHATテーブル
| column   | type   | options     |
| -------- | ------ | ----------- |
| Nickname | string | null: false |
| Text     | string | null: false |

### Association


## PREFECTURE テーブル
| column     | type    | options     |
| ---------- | ------- | ----------- |
| Prefecture | integer | null: false |

### Association
- belongs_to_active_hash :prefecture

## CHECKLIST テーブル
| column      | type      | options     |
| ----------- | --------- | ----------- |
| Item_name   | string    | null:false  |
| User        | reference | null: false |
| Description | string    |             |

### Association

## RANDOM PREFECTURE
| データベースには保存しません | type    | options     |
| ----------------------- | ------- | ----------- |