## Musicsource Database Design

## users table

|Column|Type|Options|
|------|----|-------|
|name|string|null: false|
|email|string|null: false, unique: true|

### Association

## profiles table

|Column|Type|Options|
|------|----|-------|
|first_name|string|null: false|
|last_name|string|null: false|
|address_prefecture|string| |
|country|string| |
|phone_number|string|unique: true|

### Association

## Cards table

|Column|Type|Options|
|------|----|-------|
|customer_id|string|null: false, unique: true|
|card_id|string|null: false, unique: true|
|user_id|references|null: false, foreign_key: true|

### Association

## Prefectures table

|Column|Type|Options|
|------|----|-------|
|prefecturs|string|null: false, active-hash|

### Association
