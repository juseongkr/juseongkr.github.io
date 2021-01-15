---
title: "GPG & Pass command cheatsheet"
date: 2020-10-06 01:00:00 -0400
categories: utils
---

### GPG: The GNU Privacy Guard
<https://gnupg.org>

### Pass: the standard unix password manager
<https://www.passwordstore.org>

## Contents
- [GPG](#gpg)
  - [Generate key](#generate_key)
  - [Show key](#show_key)
  - [Encrypt data](#encrypt_data)
  - [Decrypt data](#decrypt_data)
  - [Export public key](#export_public_key)
  - [Export private key](#export_private_key)
  - [Import private key](#import_private_key)
- [Pass](#pass)
  - [Init pass](#init_pass)
  - [Import pass](#import_pass)

## <a id="gpg" style="color: black;">GPG</a>

### <a id="generate_key" style="color: black;">Generate key</a>
```$ gpg --gen-key ```

### <a id="show_key" style="color: black;">Show key</a>
```$ gpg --list-keys ```

### <a id="encrypt_data" style="color: black;">Encrypt data</a>
```$ gpg --output <output> --encrypt --recipient <key-id> <input> ```

### <a id="decrypt_data" style="color: black;">Decrypt data</a>
```$ gpg --output <output> --decrypt <input> ```

### <a id="export_public_key" style="color: black;">Export public key</a>
```$ gpg --output <output> --armor --export username@email.com ```

### <a id="export_private_key" style="color: black;">Export private key</a>
```$ gpg --output <output> --armor --export-secret-key username@email.com ```

### <a id="import_private_key" style="color: black;">Import private key</a>
```$ gpg --import <input> ```

## <a id="pass" style="color: black;">Pass</a>

### <a id="init_pass" style="color: black;">Initi pass</a>
```$ pass init <private-key> ```

### <a id="import_pass" style="color: black;">Import pass</a>
```$ pass git clone ssh://<username>@<location> ``` <br />
```$ pass git remote set-url origin <username>@<location> ```
