# Bài luận triết học: Chủ nghĩa duy vật thời kì cổ đại

Chủ đề: **Chủ nghĩa duy vật thời kì cổ đại: Nội dung, giá trị và hạn chế.**

## Yêu cầu

- **TeX Live** (đã cài `texlive-full`)
- **LaTeX Workshop** (VS Code/Cursor)

## Biên dịch

Dự án dùng **XeLaTeX** để hỗ trợ tiếng Việt Unicode.

### Cách 1: LaTeX Workshop (VS Code/Cursor)

- Mở `main.tex`, nhấn **Ctrl+Alt+B** (Windows/Linux) hoặc **Cmd+Option+B** (macOS) để build.  
- Hoặc: Command Palette (**Ctrl+Shift+P** / **Cmd+Shift+P**) → gõ **Build LaTeX project** → Enter.  
- Muốn đổi recipe: Command Palette → **LaTeX Workshop: Build with recipe** → chọn **latexmk (xelatex)** hoặc **latexmk**.

**Lưu ý**  
- Cần cài extension **LaTeX Workshop** (James-Yu) trong Cursor/VS Code.  
- Trên máy cần có `latexmk` và `perl` (TeX Live thường đã kèm).  
- Nếu project dùng thư mục ra file riêng (ví dụ `%OUTDIR%`), có thể chỉnh `latex-workshop.latex.outDir` trong settings cho đúng.

### Cách 2: Dòng lệnh

```bash
cd /home/ubuntu/Projects/philosophy
latexmk
# hoặc
xelatex main.tex
biber main
xelatex main.tex
xelatex main.tex
```

## Cấu trúc

- `main.tex` — nội dung bài luận
- `references.bib` — tài liệu tham khảo (trích từ sách trong thư mục `books`)
- `books/` — tài liệu tham khảo PDF (không đưa vào repo nếu nặng)

## Tài liệu tham khảo (trong `books/`)

- Nguyễn Tiến Dũng, *Lịch sử triết học phương Tây*
- Dagobert D. Runes (Phạm Văn Liễn dịch), *Lịch sử triết học*
- Ôn Hải Minh, *Tư tưởng triết học Trung Quốc*
