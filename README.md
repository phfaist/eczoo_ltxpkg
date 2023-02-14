# Link to Error Correction Zoo from LaTeX documents

Ever wished you could simply directly link to pages on the Error Correction Zoo
from your papers?  Here's the package that enables you to do so easily.


## Quick Instructions:

1. Drop the [`eczoo.sty`](https://raw.githubusercontent.com/phfaist/eczoo_ltxpkg/main/eczoo.sty)
file on its own next to your manuscript source file;

2. Include the package as usual:

        \usepackage{eczoo}
    
3. Link to a code page with `\eczoo{surface}` or `\eczoo[Surface code]{surface}`.


## Available commands:


- `\eczoo[text]{code_id}` — place a link to a specific code on the error
  correction zoo.  The main argument should be the code ID (e.g., `surface` or
  `qldpc`, see the code identifier used in the URL address bar).  The optional
  argument can be used to include text in your link.
  
- `\eczooIcon` — place the Error Correction Zoo icon in your document at the
  default size.
  
- `\EczooIconSetScale{1.3}` — set the scale of the Error Correction Zoo icon.
  The scale is applied to the base height, which by default is a function of the
  current font size.
  
- `\EczooIconSetBaseHeight{12pt}` — set the reference base height of the icon.
  By default, this is a function of the current font size.  You can fix a
  dimension here to avoid having the icon size scale with the font size.
  
- `\EczooIconSetDefaults` — reset icon sizing options to the original defaults.

