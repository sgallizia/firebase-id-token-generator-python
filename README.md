# Firebase ID Token Generator - Python
Python script for generating [Firebase ID and refresh tokens](https://firebase.google.com/docs/auth/users#auth_tokens) 
from a user ID (UID). Useful for testing & debugging. 

ID tokens last for 1 hour (set by Firebase).

## Setup

1. Run
```
pip install -r requirements.txt
```
2. Fill out the configuration constants in get_firebase_id_token.py

## Usage
As an import (returns a dict):
```python
import firebase_token_generator

uid = "Firebase user id"
print firebase_token_generator.get_token(uid)

```

Command line (prints only the ID token):
```commandline
$ python firebase_token_generator.py <UID>
```