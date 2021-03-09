# Catatan Deployment

untuk build aplikasi NextJS, tambahkan perintah di `package.json`:

```json
"scripts": {
  "build": "node ./test-migration.js && next build",
  "export": "next export",
}
```

kemudian, jalankan perintah

```bash
npm run build && npm run export
```

✅ jika proses build berhasil, output yg diberikan:

> export successfully

❌ jika gagal, ada 3 sebab kemungkinan, karena menggunakan:

1. getInitialProps
2. getServerSideProps
3. getStaticPaths dengan return fallback : true

---

# Deploy ke github

klik menu `Action`

![](md/01.png)

scroll ke bawah, kemudian tekan tombol `More continuous integration workflows...`
(![](md/02.png))

pilih `Node.js` dan tekan <kbd>Setup this workflow</kbd>
(![](md/03.png))
