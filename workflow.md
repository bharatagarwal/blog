# Workflow breakthroughs:

I'm testing a new workflow for reading technical books in PDF format:
- Do a thorough cleanup using PDFExpert.
- Convert to text using pdf2text
- Fix linebreaks using `par -w 1000 -s`
- Split into 6k sized chunks using `split -b 6k`
- Using the prompt 'rewrite like hemingway. break into bullet points'
	- make parallel calls to `sgpt`
- Consolidate files