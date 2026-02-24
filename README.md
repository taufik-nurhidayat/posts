- Gunakan struktur ini agar konten bisa langsung dipakai di `portfolio/src/content`:

	- `content/blog/[group]/[slug]/[slug].id.md`
	- `content/blog/[group]/[slug]/[slug].en.md`

- Saat di-sync ke project portfolio:

	- `content/blog` -> `portfolio/src/content/blog`
	- `content/authors` -> `portfolio/src/content/authors`

- Frontmatter minimal untuk post:

	```md
	---
	translationKey: your-key
	slug: your-slug
	title: Judul Post
	date: 2026-02-24T10:00:00.000+00:00
	excerpt: Ringkasan singkat
	authorId: taufik-nurhidayat
	tags: tag1, tag2
	image: your-slug.id.webp
	---
	```

- Gambar thumbnail boleh:

	- File lokal di folder post yang sama (disarankan), contoh `image: your-slug.id.webp`
	- URL eksternal, contoh `image: https://example.com/image.jpg`

- Opsional: data author untuk portfolio bisa ditambahkan di `content/authors/[id].md` dengan format:

	```md
	---
	id: taufik-nurhidayat
	name: Taufik Nurhidayat
	role: Author
	bioEn: English bio
	bioId: Bio Indonesia
	avatar: taufik-nurhidayat.png
	color: bg-[#FFE66D]
	---
	```

