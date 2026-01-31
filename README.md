# GetStarted

[Official Site](https://rubyredstatesblues.github.io/GetStarted/)

Our organization stands firmly against **fascism and communism**, two extremist ideologies that—despite surface differences—both rely on authoritarian control, suppression of individual freedoms, and the subordination of people to rigid state or party power, leading historically to oppression, economic stagnation, and human suffering. We champion a **pro-globalist** vision: interconnected nations cooperating through open trade, multilateral institutions, shared democratic values, and rules-based international order to foster peace, prosperity, and innovation that transcend narrow nationalisms or collectivist dogmas. At the same time, we reject **voodoo economics**—the discredited supply-side fantasy of massive tax cuts for the wealthy and corporations magically paying for themselves through unchecked "trickle-down" growth—which repeatedly fuels inequality, balloons deficits, and undermines sustainable public investment without delivering broad-based benefits. Instead, we advocate evidence-based, inclusive economic policies that harness global markets while ensuring fair rules, strong social safety nets, and responsible fiscal stewardship to build a freer, more equitable world for all.


# Markdown

Markdown is a lightweight markup language used to format text using simple, human‑readable symbols. It’s popular because you can write plain text and still produce clean, structured documents—perfect for notes, documentation, websites, and README files on GitHub.

## Convert Mirosoft Documents to Markdown

* [How to Convert a Word Document to Markdown for Free using Pandoc](https://www.youtube.com/watch?v=HPSK7q13-40)
* [Download Software](https://github.com/jgm/pandoc)

That command is a compact little powerhouse, and each piece plays a
specific role. Breaking it down makes the whole thing feel much more
intuitive.

``` bash
pandoc -t gfm --extract-media . "fan guide.docx" -o main.md
```

**What the command does**

It converts a Word document (fan guide.docx) into a Markdown file
(main.md) using Pandoc, while also extracting any embedded images or
media into a separate folder.

**Breakdown of each part**

**pandoc**

- The universal document converter. It reads one format and outputs
  another.

**-t gfm**

- Sets the **target format**.

- gfm stands for **GitHub‑Flavored Markdown**.

- This ensures the output Markdown uses GitHub’s syntax rules (tables,
  fenced code blocks, task lists, etc.).

**--extract-media .**

- Tells Pandoc to extract all embedded media (images, audio, etc.) from
  the .docx file.

- The . means “put the extracted media in the current directory.”

- Pandoc will create a folder like media/ or fan_guide/media/ depending
  on the document.

**"fan guide.docx"**

- The **input file**.

- Quoted because it contains a space.

**-o main.md**

- The **output file**.

- Pandoc writes the converted Markdown to main.md.

**Summary**

You’re converting a Word document into GitHub‑Flavored Markdown and
pulling out all images/media into a folder in the current directory.

If you want, I can also explain how to customize the output, clean up
the media folder, or automate this for multiple files.

---
