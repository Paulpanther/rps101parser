# RPS101Parser

Parses contents of https://www.umop.com/rps101/1.htm (and all following sides)

The contents of all sides are written to `out/101.json`.
Images are downloaded to `out/symbols/<id>.png`.

Thank you to David C. Lovelace for creating the website

### Usage
1. Install dependencies with `pip install -r requirements.txt`
2. Run the script with `python parser.py` (Requires Python 3)

### Json Structure
```json
[
 {
  "id": "<number>",
  "title": "<string>",
  "img": "<path/to/img.png>",
  "compares": [
   {
    "verb": [], 
    "other_gesture_id": "<number>"
   }
  ]
 }
]
```
`verb`: First entry is words before other, second is words after other
