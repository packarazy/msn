## actualizar token

```
gpg --batch --yes --passphrase "MiContraseñaSegura" --symmetric --cipher-algo AES256 token
```

## ver token por consola

```
gpg --batch --yes --passphrase "MiContraseñaSegura" --decrypt token.gpg
```

## desifrar token.gpg
```
gpg --batch --yes --passphrase "MiContraseñaSegura" --output archivo_descifrado.txt --decrypt archivo.txt.gpg
```
