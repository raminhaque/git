# Kom igång med Git på Mac 🚀

> För dig som aldrig har använt Git förut.

## Vad är Git?

Git = **sparpunkter för dina filer**, som i ett tv-spel.
GitHub = webbsidan där du **laddar upp** dem.

## 1. Installera

```
git --version
```

Saknas Git? Klicka **Installera** i rutan som dyker upp.

## 2. Berätta vem du är

```
git config --global user.name "Ditt Namn"
git config --global user.email "din@mejl.se"
```

## 3. Skapa ett repo (projektmapp)

```
mkdir git
cd git
git init
```

## 4. Spara en version

```
git add README.md
git commit -m "Skapat README"
```

| Status | Färg i `git status` | Betyder |
|---|---|---|
| untracked | 🔴 röd | Git ser filen men sparar den inte |
| staged | 🟢 grön | Vald till nästa sparpunkt |
| committed | – | Sparad! |

## 5. Ladda upp till GitHub

1. Skapa ett tomt repo på github.com (kryssa **inte** i README)
2. Koppla ihop och ladda upp:

```
git remote add origin https://github.com/DITT-NAMN/git.git
git push -u origin main
```

> 💡 **Lösenord?** Använd en *token*, inte ditt vanliga lösenord.
> GitHub → Settings → Developer settings → Tokens (classic) → kryssa i `repo`

## Fusklapp

| Kommando | Gör |
|---|---|
| `git status` | Visar läget |
| `git add fil` | Väljer fil |
| `git commit -m ""` | Sparar |
| `git push` | Laddar upp |
| `git log` | Visar historik |