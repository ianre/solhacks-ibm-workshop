# Knowledge Base Files

This folder contains the sample workshop documents used by the two specialist agents.

## Use these during the workshop

Upload the four PDFs in [pdf](pdf):

- [pdf/scholarships-overview.pdf](pdf/scholarships-overview.pdf)
- [pdf/scholarship-faq.pdf](pdf/scholarship-faq.pdf)
- [pdf/campus-resources-guide.pdf](pdf/campus-resources-guide.pdf)
- [pdf/campus-resources-faq.pdf](pdf/campus-resources-faq.pdf)

## Edit these if you want to customize the workshop

The editable source versions live in [source](source):

- [source/scholarships-overview.md](source/scholarships-overview.md)
- [source/scholarship-faq.md](source/scholarship-faq.md)
- [source/campus-resources-guide.md](source/campus-resources-guide.md)
- [source/campus-resources-faq.md](source/campus-resources-faq.md)

After editing the source files, regenerate the PDFs:

```powershell
python scripts/build_knowledge_pdfs.py
```

## Important

These documents are sample content for a live workshop. They should not be presented as official scholarship, financial aid, or campus policy information.
