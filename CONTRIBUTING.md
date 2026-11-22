# Panduan kontribusi

## Alur kerja

`main` dilindungi: semua perubahan masuk lewat pull request.

1. Buat branch dari `main`:
   `git switch -c feat/nama-fitur`
2. Commit kecil dan jelas, satu topik per commit.
3. Push branch dan buka PR ke `main`.
4. Minta review minimal satu orang. Setelah disetujui, merge dengan **squash**.
5. Hapus branch setelah merge.

## Penamaan branch

| Awalan | Untuk |
|---|---|
| `feat/` | fitur baru |
| `fix/` | perbaikan bug |
| `docs/` | dokumentasi |
| `chore/` | tooling, dependensi, config |

## Commit

Format: `tipe(lingkup): ringkasan`

Contoh: `fix(daemon): tolak perintah startup tak dikenal`

## Review

- Reviewer mengecek logika dan dampak, bukan gaya penulisan.
- Perubahan yang mengubah perilaku sebaiknya disertai tes.
- Jangan merge PR milik sendiri tanpa review orang lain.
