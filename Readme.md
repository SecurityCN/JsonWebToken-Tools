JsonWebToken-Tools

## jwt2john.py
JWT to john 

## jwt-crack.py
JWT Signature Crack

## jwt-decoder.py

Decodes the value of JWT to jogn 
.

```
$ python3 jwt-decoder.py "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJqd3QiOiJwd24ifQ.4pOAm1W4SHUoOgSrc8D-J1
YqLEv9ypAApz27nfYP5L4"


[#] JWT Header:
{"alg": "HS256", "typ": "JWT"}

[#] JWT Value:
{"jwt": "pwn"}
```

---

## jwt-any-to-hs256.py

Generates a new JWT that is signed with HS256 with the same payload value of a provided JWT.

```
python3 jwt-any-to-hs256.py "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJqd3QiOiJwd24ifQ.4pOAm1W4SHUoOgSrc
8D-J1YqLEv9ypAApz27nfYP5L4"


[#] Generated JWT:
eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJqd3QiOiJwd24ifQ.WqY6R5zmscIx_6ZFwSASHZ_1zbqih_IdtLv_S2Pj028
```

---

## jwt-mimicker.py

Generates a new unsigned JWT with the same payload value of a provided JWT.

```
python3 jwt-mimicker.py "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJqd3QiOiJwd24ifQ.4pOAm1W4SHUoOgSrc8D-J
1YqLEv9ypAApz27nfYP5L4"


[#] Generated unsigned JWT:
eyJ0eXAiOiJKV1QiLCJhbGciOiJub25lIn0.eyJqd3QiOiJwd24ifQ.
```

---
