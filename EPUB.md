# Build the EPUB editions

This fork maintains Simplified Chinese (`book/`) and English (`book-en/`).

Install Pandoc, Poppler (`pdftoppm`), and optionally EPUBCheck. Build the corresponding PDF first; its first page becomes the EPUB cover.

```bash
./build_epub.sh all
# Or build one edition:
./build_epub.sh zh-CN
./build_epub.sh en
```

Each EPUB is written beside its PDF and is ignored by Git. EPUBCheck validates generated books when installed.
