# Quarto Book Template

Welcome to the Quarto Book Template repository! This template provides a solid foundation for authors looking to create and publish their books using [Quarto](https://quarto.org/), an open-source scientific and technical publishing system.

## Features

- **Multi-format Output:** Generate books in HTML, PDF, EPUB, and Microsoft Word formats.
- **Easy Chapter Management:** Organize your book with individual chapter files.
- **Customizable Configuration:** Tailor your book's appearance and structure via the `_quarto.yml` file.
- **Cross-referencing:** Automatically number chapters and sections for easy cross-referencing.
- **Bibliography Support:** Manage references with a `references.bib` file.
- **Interactive Elements:** Incorporate code, equations, and interactive components seamlessly.

## Getting Started

### Prerequisites

- **Quarto:** Ensure you have the latest version of Quarto installed. Download it from the [Quarto Downloads Page](https://quarto.org/docs/get-started/).

### Installation

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/yourusername/quarto-book-template-en.git
   cd quarto-book-template-en
   ```

2. **Install Dependencies:**
   If your book relies on specific packages or extensions, install them as needed. For example, to install TinyTeX:
   ```bash
   quarto install tinytex
   ```

3. **Render the Book:**
   ```bash
   quarto render
   ```

### PDF/LaTeX Rendering with Custom Preamble

The `preamble.tex` file includes several key elements that customize the PDF output for your book. Here's an overview of its main components:

- **Typographical Packages:**
  - **microtype:** Enhances the overall typography by improving character spacing and hyphenation.
  - **setspace:** Manages line spacing within the document to ensure readability.
  - **fontspec:** Enables the use of OpenType fonts, allowing for greater flexibility in font selection.

- **Typography Settings:**
  - **Paragraph Formatting:** Adjusts paragraph spacing and indentation to create a clean and consistent layout.
  - **Line Spread:** Sets the line spacing to 1.3 for improved readability.
  - **Hyphenation Control:** Configures hyphenation penalties to manage word breaks effectively.

- **Custom Commands for Title Pages:**
  - **Title Definitions:** Defines custom commands like `\titleoriginal`, `\subtitleoriginal`, and `\press` to standardize title page information.
  - **Custom Title Page Layout:** Implements specialized commands (`\halftitlepage`, `\titleM`, and `\copyrightpage`)
    to create aesthetically pleasing title and copyright pages.

- **Physical Document Setup:**
  - **Page Dimensions:** Sets the stock size and trimmed size to 210mm by 148mm, suitable for standard book formats.
  - **Margins and Binding:** Configures left and right margins, top and bottom margins, and binding offset to ensure proper page layout.

- **Font Configuration:**
  - **Main and Sans Fonts:** Specifies the main serif font (`stone-serif`) and sans-serif font (`stone-sans`) with detailed settings for various font styles and weights.
  
- **Header and Footer Customization:**
  - **Page Styles:** Defines custom page styles (`mystyle` and `plain`) to control the appearance of headers and footers, including page numbers and section titles.
  - **Running Headers:** Sets up running headers to display chapter titles and page numbers appropriately on even and odd pages.

- **Table of Contents (TOC) Formatting:**
  - **TOC Style:** Customizes the appearance of the table of contents using the `tocloft` package, adjusting fonts, indentation, and spacing for sections and chapters.

- **Footnote Redefinition:**
  - **Footnote Layout:** Alters the default footnote formatting to improve the alignment and appearance of footnotes within the document.

- **Layout Checks and Fixes:**
  - Ensures that the document layout adheres to the specified configurations and makes necessary adjustments to maintain consistency.

By incorporating these elements, the `preamble.tex` file provides comprehensive control over the document's appearance, ensuring that the final PDF meets your design and formatting standards.

``` 

### Continuous Integration (CI)
